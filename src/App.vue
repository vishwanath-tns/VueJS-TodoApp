<template>
  <div id="app">
    <div class="grid bg-gray-100 grid-cols-4 gap-2">
      <div class="flex text-center bg-gray-100 justify-left p-2 pl-5">
        
        <svg viewBox="0 0 20 20" fill="indigo" class="clipboard-list w-12 h-12"><path d="M9 2a1 1 0 000 2h2a1 1 0 100-2H9z"></path><path fill-rule="evenodd" d="M4 5a2 2 0 012-2 3 3 0 003 3h2a3 3 0 003-3 2 2 0 012 2v11a2 2 0 01-2 2H6a2 2 0 01-2-2V5zm3 4a1 1 0 000 2h.01a1 1 0 100-2H7zm3 0a1 1 0 000 2h3a1 1 0 100-2h-3zm-3 4a1 1 0 100 2h.01a1 1 0 100-2H7zm3 0a1 1 0 100 2h3a1 1 0 100-2h-3z" clip-rule="evenodd"></path></svg>
        <h1 class="pl-2 text-left text-3xl inline-block">Todo App</h1>
      </div>
      <div class="flex flex-row items-stretch h-14 justify-between col-start-4 p-5 text-xl">
        <div>
          <router-link to='/'> Home </router-link>
        </div>
        <div>
          <router-link to='/signin'> Sign In </router-link>
        </div>
        <div>
          <router-link to='/About'> About </router-link>
        </div>
        
      </div>
      <div class="col-start-5 rounded-md p-2">
        <a href="#" class="w-auto flex justify-center px-8 py-3 text-base leading-6 font-medium rounded-md text-white bg-indigo-600 hover:bg-indigo-500 focus:outline-none focus:border-indigo-700 focus:shadow-outline-indigo transition duration-150 ease-in-out md:py-4 md:text-lg md:px-10">
          Register
        </a>
      </div>
    </div>
    
    <div class="">
      <router-view class="" :key="$route.path"/>
    </div>
    
  </div>
</template>
<script>


export default {
  components: {
    
  }
}
</script>
<style src="./assets/css/tailwind.css">

</style>
