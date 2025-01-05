<template>
  <CustomButton btn-type="primary" @click="exportPdf" style="margin-bottom: 10px;">
    Export resume as PDF
  </CustomButton>
</template>

<script>
import CustomButton from './CustomButton.vue';
import html2pdf from 'html2pdf.js'; // Ensure this is installed via npm/yarn

export default {
  components: {
    CustomButton,
  },
  props: {
    resumeFormat: {
      type: String,
      default: 'a4', // Default to 'a4' if not provided
    },
  },
  methods: {
    exportPdf() {
      const unit = this.resumeFormat === 'a4' ? 'mm' : 'in';

      // Ensure the DOM element exists
      const resume = document.getElementById('resume');
      if (!resume) {
        console.error("The element with ID 'resume' was not found.");
        return;
      }

      // PDF configuration
      const pdfConfig = {
        margin: 0,
        filename: 'resume.pdf', // Add the `.pdf` extension for clarity
        jsPDF: {
          unit: unit,
          format: this.resumeFormat,
          orientation: 'portrait',
        },
      };

      // Use html2pdf to export the element
      html2pdf()
        .set(pdfConfig)
        .from(resume)
        .save()
        .then(() => {
          console.log('PDF export successful!');
        })
        .catch((error) => {
          console.error('Error exporting PDF:', error);
        });
    },
  },
};
</script>
