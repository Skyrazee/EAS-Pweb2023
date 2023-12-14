<template>
  <div>
    <h1>Formulir Registrasi Lomba</h1>
    <App />
  </div>
</template>

<script>
import App from '~/components/App.vue';

export default {
  components: {
    App,
  },
};
</script>

<style>
/* Styling for your page goes here */
</style>

  <div>
    <CheckStatus />
  </div>
</template>

<script>
import CheckStatus from '~/components/CheckStatus.vue';

export default {
  components: {
    CheckStatus,
  },
};
</script>

<style>
/* Add your styling for the CheckStatus page */
</style>

  <div>
    <h1>Formulir Registrasi Lomba</h1>
    <App />

    <router-link to="/check-status">Cek Status Pendaftaran</router-link>
  </div>
</template>

<script>
import App from '~/components/App.vue';

export default {
  components: {
    App,
  },
};
</script>

<style>
/* Styling for your page goes here */
</style>

