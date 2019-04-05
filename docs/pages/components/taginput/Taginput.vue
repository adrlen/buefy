<template>
  <div>
    <Example
      :component="ExAutocomplete"
      :code="ExAutocompleteCode"
      title="Autocomplete"
      vertical
    >
      <p>
        To have autocomplete functionality, add the
        <code>autocomplete</code> prop. You can add any prop from
        <router-link to="/documentation/autocomplete">Autocomplete</router-link>
        API.
      </p>
    </Example>

    <ApiView :data="api" />
  </div>
</template>

<script>
import api from "./api/taginput";

import ExSimple from "./examples/ExSimple";
import ExSimpleCode from "!!raw-loader!./examples/ExSimple";

import ExAutocomplete from "./examples/ExAutocomplete";
import ExAutocompleteCode from "!!raw-loader!./examples/ExAutocomplete";

import ExTemplatedAutocomplete from "./examples/ExTemplatedAutocomplete";
import ExTemplatedAutocompleteCode from "!!raw-loader!./examples/ExTemplatedAutocomplete";

import ExLimit from "./examples/ExLimit";
import ExLimitCode from "!!raw-loader!./examples/ExLimit";

import ExState from "./examples/ExState";
import ExStateCode from "!!raw-loader!./examples/ExState";

import ExType from "./examples/ExType";
import ExTypeCode from "!!raw-loader!./examples/ExType";

import ExSize from "./examples/ExSize";
import ExSizeCode from "!!raw-loader!./examples/ExSize";

import ExModifier from "./examples/ExModifier";
import ExModifierCode from "!!raw-loader!./examples/ExModifier";

import ExValidation from "./examples/ExValidation";
import ExValidationCode from "!!raw-loader!./examples/ExValidation";

export default {
  data() {
    return {
      api,
      ExSimple,
      ExAutocomplete,
      ExTemplatedAutocomplete,
      ExLimit,
      ExState,
      ExType,
      ExSize,
      ExModifier,
      ExValidation,
      ExSimpleCode,
      ExAutocompleteCode,
      ExTemplatedAutocompleteCode,
      ExLimitCode,
      ExStateCode,
      ExTypeCode,
      ExSizeCode,
      ExModifierCode,
      ExValidationCode
    };
  }
};
</script>
