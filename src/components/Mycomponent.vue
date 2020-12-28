<template>
  <div class="conatiner">
    <div class="user-card">
      <h1>Научу зарабатывать от 50 000р. в час</h1>
      <div class="main-information flex">
        
        <div class="info">
          <h2>{{ getAuthorFullName }}</h2>

          <strong>Бизнес-коуч</strong>
          <li v-for="item in items" :key="item.message">
             {{ item.message }}
          </li>
          <ul class="list">
            <li>Учу делать РЕАЛЬНЫЕ бабки, на себя просто не хватило времени</li>
            <li>НЕ знаю, что такое "Успешный Успех", но знаю, что нужно ТЕБЕ!</li>
            <li>Пообещал, что побреюсь, когда кого-нибудь ОБМАНУ.</li>
          </ul>
        </div>
      </div>
    </div>
  </div>
  
 
</template>

<script>
export default {
  name: 'UserCard',
  data() {
    return {
      firstName: 'Игнатий',
      secondName: 'Иларионович',
      lastName: 'Богатов',
      items: [
      { message: 'Foo' },
      { message: 'Bar' }
    ]
    }
  },
  computed: {
    getAuthorFullName() {
      return `${this.firstName} ${this.secondName} ${this.lastName}`.toUpperCase()
    }
  },
  methods: {
   
  },
    

  
  watch: {
    
    
  }
}
</script>


