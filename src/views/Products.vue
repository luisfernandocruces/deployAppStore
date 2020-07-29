<template>
    <v-container>
        <v-row>
            <h1>Estos son los celulares</h1>
        </v-row>
        <v-row>
            <v-col
        v-for="n in 3"
        :key="n"
        cols="12"
        sm="4"
      >
         <v-card
    class="mx-auto"
    max-width="400"
  >
    <v-img
      class="white--text align-end"
      height="200px"
      src="https://cnet3.cbsistatic.com/img/k8D-4A5ls8OzDmPyImx7VF_0AUU=/2020/04/07/5a7fcdbd-b99a-4f9b-9a33-25fc1db4dfd5/galaxy-s20.jpg"
    >
    </v-img>
    <v-card-title>Samsung S20</v-card-title>

    <v-card-subtitle class="pb-0">$4.000.000</v-card-subtitle>

    <v-card-text class="text--primary">
      <div>El mejor celular gama alta de Samsung</div>
    </v-card-text>

    <v-card-actions>
      <v-btn
        color="orange"
        text
      >
        Share
      </v-btn>

      <v-btn
        color="orange"
        text
      >
        Explore
      </v-btn>
    </v-card-actions>
  </v-card>
      </v-col>
        </v-row>
    </v-container>
</template>

<script>
export default {

}
</script>

<style>

</style>