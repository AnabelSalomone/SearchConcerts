<template>
<div class="container">
<ul class="collection">
    <li class="collection-item avatar" v-for="item in datas.shows">
      <img :src="item.img" alt="" class="circle">
      <span class="title">{{item.titre}}</span>
      <p>Lieu: {{item.lieu.nom}} <br>
        Adresse: {{item.lieu.adresse}}, {{item.lieu.arrondissement}}, Lyon<br>
				Prix: {{item.prix}} €
      </p>
      <a href="#!" class="secondary-content"><i class="material-icons">grade</i></a>
    </li>
		</ul>
</div>

</template>

<script>
import {Store} from '@/Store.js'


export default {
	name: 'list',
	data(){
		return{
			datas: Store.datas
		}
	}
  // computed: {
  //   datas(){
  //     return Store.datas.shows
  //   }
  // }
}
</script>
