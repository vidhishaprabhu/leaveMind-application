<template>
  <div class="sidebar">
    <h4>LeaveMind</h4>
    <img src="@/assets/main-logo.png" alt="Logo" class="logo" />
    <router-link to="/dashboard" class="nav-link"><HomeOutlined style="color:white;padding-right:12px"/>Dashboard</router-link>
    <router-link to="/request-leave" class="nav-link">Request Leave</router-link>
    <router-link to="/leave-history" class="nav-link">Leave History</router-link>
    <button class="logout-btn" @click="logout"><PoweroffOutlined/> Logout</button>
  </div>
</template>
<script>

import {
  HomeOutlined,
  PoweroffOutlined,
   FileAddOutlined
 
} from '@ant-design/icons-vue'
export default{
  name:'AppSidebar',
  components:{
HomeOutlined,
PoweroffOutlined,
 FileAddOutlined
  }
  

}
</script>


<style scoped>
*{
  margin: 0;
  padding: 0;
}
.logo {
  width: 100px;        
  height: auto;       
  display: block;     
}
.sidebar {
   font-family: 'Poppins', sans-serif;
  height: 100vh;
  width: 220px;
  background-color: #111827; /* Dark Slate Blue (good for sidebars) */
  color: white;
  padding: 20px;
  position: fixed;
  box-shadow: 2px 0 8px rgba(0, 0, 0, 0.2);
}
.nav-link {
  display: block;
  margin: 12px 0;
  color: white;
  text-decoration: none;
  font-weight: 500;
}
.nav-link:hover {
  background-color: #334155; /* Slightly lighter hover */
  padding-left: 10px;
  transition: 0.3s;
}
.logout-btn {
  margin-top: 20px;
  background-color: transparent;
  border: 1px solid white;
  color: white;
  padding: 8px 12px;
  cursor: pointer;
  width: 100%;
}
.logout-btn:hover {
  background-color: #474869;
}
</style>
