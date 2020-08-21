<template>
  <section class="main-wrapper">
<Headertext/>
<Flytxt/>
<Banner/>
<Txt show="true" head="Get ready for a unique experience" desc="Fishtripr has partnered with fishing guides and local experts all over the world to help you craft the ultimate fishing experience or simply catch your first fish!"/>
<Video/>
 <Txt show="true" head="Fishing for every budget and style" desc="Family getaway, team building, fishing immersion? Narrow down your search using our tour categories, and tell us what would make your perfect trip."/>
<Loader />
<Txt head="Our guests' stories"/>
<Guests/>
<Employee/>
<Subscribe/>
</section>
</template>

<script>
import Headertext from '@/components/header-part/Headertext'
import Flytxt from '@/components/flytext-part/Flytxt'
import Banner from '@/components/banner-part/Banner'
import Video from '@/components/video-part/Video'
import Txt from '@/components/Txt'
import Loader from '@/components/loader-part/Loader'
import Guests from '@/components/guests-part/Guests'
import Employee from '@/components/employee-part/Employee'
import Subscribe from '@/components/subscribe-part/Subscribe'
export default {
components:{
  Headertext,
  Flytxt,
  Banner,
  Video,
  Txt,
  Loader,
  Guests,
  Employee,
  Subscribe
}
}
</script>

<style lang="scss" scoped>
.main-wrapper {
  width: 100%;
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  margin-top: 150px;
}
</style>