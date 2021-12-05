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
			
			<div class="profile-bio">

				<p>{{profilePosition}} at {{profileDept}}</p>
				<p>Incharge of {{profileClub}}</p>

			</div>

			<div class="profile-stats">
				<ul>
					<li><span class="profile-stat-count">{{profilePostNos}}</span> <span class="profile-stat-caption">Posts</span></li>
					<li><span class="profile-stat-count">{{profileSeminarNos}}</span> <span class="profile-stat-caption">Seminars</span></li>
					<li><span class="profile-stat-count">{{profileCourseNos}}</span> <span class="profile-stat-caption">Courses</span></li>
				</ul>

			</div>


		</div>

	</div>

</header>
</template>

<script>
export default {
    data(){
        return{
            profilePicURL:'https://pbs.twimg.com/profile_images/1295112038096629760/3eCOaKDb_400x400.jpg',
            profileName:'Simon Sinek',
            profileDept:'Department of Information Technology',
            profilePostNos:'10',
            profileSeminarNos:'55',
            profileCourseNos:'12',
            profilePosition:'Assistant Professor',
            profileClub:'Readers Club'
        }
    }
}
</script>

<style scoped src="../assets/styles/profile-page-lay.css">
/* There's a CSS File in src>assets>styles with Same File Name separated with Hyphens */

</style>