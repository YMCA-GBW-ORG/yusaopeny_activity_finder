<template>
  <div class="search-form-component">
    <input
      v-model="searchKeywords"
      type="text"
      class="form-control"
      :placeholder="'Keyword(s)' | t"
      @keyup.enter.prevent="runSearch"
    />
    <button class="btn" @click.stop.prevent="runSearch">
      <span class="fa fa-search" :aria-label="'Search' | t"></span>
    </button>
  </div>
</template>

<script>
export default {
  name: 'SearchForm',
  props: {
    value: {
      type: String,
      required: true
    }
  },
  data() {
    return {
      searchKeywords: this.value
    }
  },
  watch: {
    value() {
      this.searchKeywords = this.value
    }
  },
  methods: {
    runSearch() {
      this.$emit('input', this.searchKeywords)
    }
  }
}
</script>

<style lang="scss">
.search-form-component {
  border: 1px solid $af-dark-gray;
  color: $af-dark-gray;
  display: flex;
  margin: 0 auto;

  .form-control {
    border: none;
    font-size: 12px !important;
    line-height: 18px;
    height: 38px;
  }

  .btn {
    background-color: $af-violet;
    color: $white;
    width: 40px;
    padding: 6px 12px;
    border: none;
    font-size: 18px;
    line-height: 1;
    border-radius: unset;

    .fa {
      font-size: 18px;
    }
  }

  ::-webkit-input-placeholder {
    font-size: 12px;
    font-style: normal;
  }
  :-moz-placeholder {
    font-size: 12px;
    font-style: normal;
  }
  ::-moz-placeholder {
    font-size: 12px;
    font-style: normal;
  }
  :-ms-input-placeholder {
    font-size: 12px;
    font-style: normal;
  }
}
</style>
