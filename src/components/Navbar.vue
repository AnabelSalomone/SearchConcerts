<template>
<nav>
    <div class="nav-wrapper red">
      <a href="#" class="brand-logo"><img src="http://greetings2015.onlylyon.com/static/img/big_logo_only1.png" style="height: 50px;;"></a>
      <ul id="nav-mobile" class="right hide-on-med-and-down black-text">
			<li><form class="col s4">
        <div class="input-field col s12">
          <i class="material-icons prefix">account_circle</i>
          <input id="icon_prefix" type="text" class="validate" v-model="datas.search">
          <label for="icon_prefix" v-if="search.length === 0"></label>
        </div>
				</form></li>
        <li class ="black-text"><a href="sass.html">Musique</a></li>
        <li class ="black-text"><a href="badges.html">Thatre</a></li>
        <li class ="black-text"><a href="collapsible.html">Danse</a></li>
      </ul>
    </div>
  </nav>
</template>

<script>
import {Store} from '@/Store.js'


export default {
	name: 'navbar',
	data(){
    return {
			datas: Store.datas,
			search: ''
    }
  }
}
</script>

<style scoped>
ul li a{
  color: black;
 }
</style>