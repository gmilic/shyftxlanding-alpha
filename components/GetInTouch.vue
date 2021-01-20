<template>
  <v-container
    fluid
    class="px-0 py-16"
  >
    <v-row>
        <v-col
            cols=12
            md=6
        >
            <v-img
                src="img/getInTouch.png"
            >
            </v-img>
        </v-col>
        <v-col
            cols=12
            md=6
        >
        <h3
            class="text-h3 my-16"
        >Get in Touch
        </h3>
        <h5
            class="text-h5 my-6"
        >
            Have more questions?<br /> 
            We're here for you 24/7.
        </h5>
          <v-form>
            <v-container>
            <v-row>
                <v-col
                cols="12"
                sm="6"
                >
                <v-text-field
                    v-model="fullname"
                    label="Full Name"
                    :rules="nameRules"
                    outlined
                    required
                    placeholder="Input your full name in here"
                ></v-text-field>
                </v-col>

                <v-col
                cols="12"
                sm="6"
                >
                <v-text-field
                    label="Email Address"
                    outlined
                    v-model="email"
                    :rules="emailRules"
                    required
                    placeholder="Input your email address in here"
                ></v-text-field>
                </v-col>
            </v-row>
            <v-row>
                <v-col
                    cols="12"
                    sm="12"
                >
                <v-textarea
                    outlined
                    name="message"
                    label="Message"
                    required
                    auto-grow
                    placeholder="Write your messages in here"
                    ></v-textarea>
                </v-col>
            </v-row>
            </v-container>
        </v-form>
        </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
    data: () => ({
      valid: false,
      fullname: '',
      nameRules: [
        v => !!v || 'Full Name is required',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail is required',
        v => /.+@.+/.test(v) || 'E-mail must be valid',
      ],
    }),
}
</script>

<style>

</style>