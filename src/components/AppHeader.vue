<script>
export default {

data() {
    return{
        links: [
            {
                label:'CHARACTERS',
                url:'#',
                current: false
            },
             {
                label:'COMICS',
                url:'#',
                current: false
            },
             {
                label:'MOVIES',
                url:'#',
                current: false
            },
             {
                label:'TV',
                url:'#',
                current: false
            },
             {
                label:'GAMES',
                url:'#',
                current: false
            },
             {
                label:'COLLECTIBLES',
                url:'#',
                current: false
            },
             {
                label:'VIDEOS',
                url:'#',
                current: false
            },
             {
                label:'FANS',
                url:'#',
                current: false
            },
             {
                label:'NEWS',
                url:'#',
                current: false
            },
             {
                label:'SHOP',
                url:'#',
                current: false
            }
            
        ]
    }
}
    
}
</script>
<template>
    <header>
                          
               
           <nav class="navbar navbar-expand-lg navbar-light bg-white">
        <div class="container">
            <a class="navbar-brand" href="#">
                <img src="../assets/dc-logo.png"height="100" />  
            </a>

            <div class="col-9">
                <ul class="navbar-nav ms-auto">
                <li v-for="link,index in links" :key="index" :class="['nav-item', link.current ? 'active' : '']">
                    <a :href="link.url"class="nav-link">{{ link.label }}</a>
                
                </li>
                
            </ul>
        </div>
        </div>
    </nav>
             
               <div class="col-12">
                    <img src="../img/jumbotron.jpg"  class="img-fluid">
                     
                </div>  
                 

            
    </header>
</template>



<style lang="scss">
   .navbar {
    box-shadow: 0 2px 4px rgba(0,0,0,.1);
}

 .navbar-nav .nav-item .nav-link {
    color: #000;
    font-weight: 600;
    text-transform: uppercase;
    padding: 0.5rem 1rem !important;
    transition: color 0.3s ease;
}

.navbar-nav .nav-item .nav-link:hover,
.navbar-nav .nav-item .nav-link:focus {
    color: #0082F9;
}

.navbar-nav .nav-item.active .nav-link {
    color: #0082F9;
}
   
        .footer-links {
            background-color: #0082F9;
            color: #fff;
            padding: 20px 0;
        }
        .footer-menu {
            background-color: #222;
            color: #fff;
            padding: 20px 0;
        }
    </style>