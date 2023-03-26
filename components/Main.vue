<template>
  <div>
    <b-form-group label="MDL file name">
      <b-form-input v-model="fileName" />
    </b-form-group>

    <b-form-group label="MDL file contents">
      <b-form-textarea v-model="fileContents" />
    </b-form-group>

    <b-button variant="primary" @click="saveFile">Save</b-button>
  </div>
</template>

<script>
export default {
  data() {
    return {
      fileName: '',
      fileContents: ''
    }
  },

  methods: {
    saveFile() {
      // Use axios or another library to save the file to the server
      // Example using axios:
      this.$axios.post('/save-file', {
        name: this.fileName,
        contents: this.fileContents
      })
      .then(response => {
        console.log(response)
      })
      .catch(error => {
        console.log(error)
      })
    }
  }
}
</script>
