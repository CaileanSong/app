<script setup lang="ts">
    const interfacename = ref('')
    const router = useRouter()
    const name = 'User Name'

    const interfaceList = [
        {id:1,name:'post1',},
        {id:2,name:'get1'},
        {id:3,name:'post2'},
        {id:4,name:'get2'},
    ]

    function search(){
        
    }



</script>

<template>
    <div 
      w="100%"
      h="100%"
      border="~  gray-200 dark:gray-700"
    >
    <div >
      <img src="" alt=""
       w="50px" h="50px" m="l-8" 
       border="~ rounded-8" 
       float="left"  >
      <p w="80%" 
       h="50px" 
       m="l-21" text="left"  
       line-height="50px"  >{{ name }}</p>
    </div>
    
    <input
      background=""
      id="input"
      v-model="interfacename"
      placeholder="search for interface"
      type="text" autocomplete="off"
      p="x-4 y-2" m="t-5" 
      text="center" bg="transparent"
      border="~ rounded gray-200 dark:gray-700"
      outline="none active:none"
      @keydown.enter="search"
    >
    <div p="x-4" display="flex" justify-content="flex-start" >
      <router-link to="path"
        display="block"   
        m="x-1"
         >
        All Request
      </router-link>
    </div>
    <div p="x-4" w="100%">
      <router-link to="path" 
        display="block"   
        text-align="left"  
       >
        Settings
    </router-link>
    </div>
      
    

    
    </div>
</template>