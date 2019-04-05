<template>
  <section>
    <b-taginput
      v-model="tags"
      :data="filteredTags"
      autocomplete
      open-on-focus
      icon="label"
      placeholder="Add a tag"
      @typing="getFilteredTags"
    >
    </b-taginput>
  </section>
</template>

<script>
const data = ['dazdazdz', 'dazdazza', 'dazda'];

export default {
  data() {
    return {
      filteredTags: data,
      isSelectOnly: false,
      tags: [],
      allowNew: false
    };
  },
  methods: {
    getFilteredTags(text) {
      this.filteredTags = data.filter(option => {
        return (
          option.user.first_name
            .toString()
            .toLowerCase()
            .indexOf(text.toLowerCase()) >= 0
        );
      });
    }
  }
};
</script>

