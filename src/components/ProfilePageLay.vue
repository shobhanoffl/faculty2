<template>
<!-- This Layout displays the Profile Info of the user -->
  <header>

	<div class="container">

		<div class="profile">
			<div class="profile-image">

				<img :src="profilePicURL">

			</div>

			<div class="profile-user-settings">

				<h1 class="profile-user-name">{{profileName}}</h1>

				<p class="profile-dept-btn">{{profileDept}}</p>


			</div>
				
			<div class="profile-stats">

				<ul>
					<li><span class="profile-stat-count">{{profilePostNos}}</span> <span class="profile-stat-caption">Posts</span></li>
					<li><span class="profile-stat-count">{{profileSeminarNos}}</span> <span class="profile-stat-caption">Seminars</span></li>
					<li><span class="profile-stat-count">{{profileCourseNos}}</span> <span class="profile-stat-caption">Courses</span></li>
				</ul>

			</div>

			<div class="profile-bio">

				<p>{{profilePosition}} at {{profileDept}}</p>
				<p>Incharge of {{profileClub}}</p>

			</div> 

		</div>

	</div>

</header>
</template>

<script>
import "@/assets/styles/profile-page-lay.css";
export default {
    data(){
        return{
            profilePicURL:'',
            profileName:'',
            profileDept:'',
            profilePostNos:'',
            profileSeminarNos:'',
            profileCourseNos:'',
            profilePosition:'',
            profileClub:''
        }
    }
}
</script>

<style scoped>
/* There's a CSS File in src>assets>styles with Same File Name separated with Hyphens */

</style>