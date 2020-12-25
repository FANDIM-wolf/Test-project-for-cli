<template>
	<div class="root">
	<label>
	Enter email:
	<input type="email" v-bind:value="email" @input="emailInput($event.target.value)" name=""> 	
	</label>
	<label>
	Enter password:
	<input type="password" v-bind:value="password" @input="passwordInput($event.target.value)" name=""> 	
	</label>
	<br>
	<button @click="count--">-</button>
	<input type="number" v-bind:value="count"  name="">
    <button @click="count++">+</button>


		
	</div>
</template>

<script >
	export default{
		name: 'Mycomponent',
		data(){
               
        return{text:"Lafore",
               email:'example@mail.ru',
               password:'12345678',
               count:0
    }
	},
	methods:{
		emailInput(value){
           this.email= value //new value of email
		},
		passwordInput(value){
			this.password = value
		}
	}

}
</script>