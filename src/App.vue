<script>
// import TopNavBar from '@/components/TopNavBar.vue'; 
import SideNav from '@/components/SideNav.vue';
import HeroSection from '@/components/HeroSection.vue';
import FooterSection from './components/FooterSection.vue';
export default{
    components:{
        // TopNavBar,
        SideNav,
        HeroSection,
        FooterSection
    }
}
</script>
<template>
   <div class="container-fluid overflow-hidden">
        <div class="row vh-100 overflow-auto">
            <!-- side Nav -->
            <SideNav></SideNav>
                <div class="col d-flex flex-column h-sm-100">
                    <main class="row overflow-auto">
                        <HeroSection/>
                    </main>
                    <FooterSection/>
                </div>
        </div>
    </div>
  <RouterView />
</template>
<style>
@media (min-width: 576px) {
    .h-sm-100 {
        height: 100%;
    }
}
</style>

