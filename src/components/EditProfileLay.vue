<template>
<!-- This is Edit Profile Layout which provides options to Edit the Profile-->
<v-app>
<div class="editprofile-wrap">
    <div class="profile">
        <v-form>
			<div class="profile-image">

				<img src="https://avatarfiles.alphacoders.com/516/51684.png" alt="">

                <div class="update-link">Change Profile Photo</div>

			</div>

			<div class="profile-user-settings">

				<v-text-field v-model="fullname" :counter="25" label="Name" prepend-icon="mdi-account-edit" required></v-text-field>

				<p class="profile-dept-btn" style="margin-top:12px;"><v-select v-model="selecteddept" :items="depts" label="Department" prepend-icon="mdi-account-details" required></v-select></p>

			</div>

			<div class="profile-bio">

				<p><v-select v-model="selectedtitle" :items="titles" label="Title" prepend-icon="mdi-badge-account-horizontal" required></v-select></p>
				<p><v-select v-model="selectedclub" :items="clubs" label="Club Involved" prepend-icon="mdi-account-group" required></v-select></p>
				<!-- <p>Asst. Professor at Department of Information Technology</p> -->

			</div>
            <div class="editprofile-btns">
                <span class="update-btn">Submit</span>
                <span class="update-link">Cancel</span>
            </div>
        </v-form>
	</div>
</div>
</v-app>
</template>

<script>
/* No Props needed since there won't be much change in the options provided */
export default {
    data:() => ({
        selecteddept:null,
        depts: ['Item 1','Item 2','Item 3','Item 4','ss','sda'],
        fullname:'',
        dept:'',
        selectedtitle:null,
        titles: ['Itesm 1','Item 2','Item 3','Item 4'],
        selectedclub:'',
        clubs:['Itesm 1','Item 2','Item 3','Item 4']
    })
}
</script>

<style scoped src="../assets/styles/edit-profile-lay.css">
/* There's a CSS File in src>assets>styles with Same File Name separated with Hyphens */
</style>