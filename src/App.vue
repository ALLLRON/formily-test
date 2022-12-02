<template>
  <FormProvider :form="form">
    <Field name="input" :component="[Input]" />
  </FormProvider>
</template>

<script>
import { Input } from "iview";
import { createForm } from "@formily/core";
import { FormProvider, Field } from "@formily/vue";

export default {
  components: { FormProvider, Field },
  data() {
    return {
      Input,
      form: createForm(),
    };
  },
};
</script>
