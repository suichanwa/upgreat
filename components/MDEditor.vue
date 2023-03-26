<template>
  <div>
    <h1>{{ fileName }}</h1>
    <b-form-group label="File name">
      <b-form-input v-model="fileName" />
    </b-form-group>
    <b-form-group label="File contents">
      <b-form-textarea v-model="fileContents" />
    </b-form-group>
    <b-button variant="primary" @click="saveFile">Save</b-button>
  </div>
</template>

<script>
export default {
  props: {
    file: {
      type: Object,
      required: true
    }
  },

  data() {
    return {
      fileName: '',
      fileContents: ''
    }
  },

  mounted() {
    // Set the initial file name and contents
    this.fileName = this.file.name
    this.fileContents = this.file.contents
  },

  methods: {
    saveFile() {
      // Emit a "save-file" event with the updated file data
      this.$emit('save-file', {
        id: this.file.id,
        name: this.fileName,
        contents: this.fileContents
      })
    }
  }
}
</script>
