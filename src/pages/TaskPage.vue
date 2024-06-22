<template>
    <div class="task-container">
      <q-page>
        <q-card class="task-card">
          <q-list bordered padding>
            <q-item v-for="taskNumber in taskNumbers" :key="taskNumber" clickable @click="goToTask(taskNumber)">
              <q-item-section>
                <q-item-label>{{ `Ini tugas ${taskNumber}, Ferina ` }}</q-item-label>
              </q-item-section>
            </q-item>
          </q-list>
        </q-card>
      </q-page>
    </div>
  </template>
  
  
  <script>
export default {
  data() {
    return {
      taskNumbers: [1, 2, 3, 4, 5, 6, 7]
    };
  },
  methods: {
    goToTask(taskNumber) {
      const taskLinks = {
        1: "https://tugas-pbk-223510431.vercel.app/",
        2: "https://tugas2-prakpbk-muhammadrevisuryandi-223510431.vercel.app/",
        3: "https://tugas3-pbk-muhammadrevisuryandi-223510431-4b.vercel.app/",
        4: "https://tugas4-muhammadrevisuryandi-223510431.vercel.app",
        5: "https://reppshop.vercel.app/",
        6: "https://t6revi.vercel.app/",
        7: "https://t7revii.vercel.app/"
      };
      window.open(taskLinks[taskNumber], '_blank');
    }
  }
};
</script>

  
<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400;500;700&display=swap');

* {
  font-family: 'Roboto', sans-serif;
}

</style>
