<template>
<v-app>
	<v-app-bar
		app
		color="blue darken-3"
		dark
		dense
	>
		<v-spacer></v-spacer>
			<router-link class="routerLink" to="/">
				<v-list-item link>
					<v-list-item-icon class="mr-2">
						<v-icon>mdi-login</v-icon>
					</v-list-item-icon>
					<v-list-item-content>
						<v-list-item-title>REST Home</v-list-item-title>
					</v-list-item-content>
				</v-list-item>
			</router-link>
			<router-link class="routerLink" to="/restAdd">
				<v-list-item link>
					<v-list-item-icon class="mr-2">
						<v-icon>mdi-login</v-icon>
					</v-list-item-icon>
					<v-list-item-content>
						<v-list-item-title>REST Add Product</v-list-item-title>
					</v-list-item-content>
				</v-list-item>
			</router-link>
			<router-link class="routerLink" to="/graphql">
				<v-list-item link>
					<v-list-item-icon class="mr-2">
						<v-icon>mdi-login</v-icon>
					</v-list-item-icon>
					<v-list-item-content>
						<v-list-item-title>GraphQL Home</v-list-item-title>
					</v-list-item-content>
				</v-list-item>
			</router-link>
			<router-link class="routerLink" to="/graphqlAdd">
				<v-list-item link>
					<v-list-item-icon class="mr-2">
						<v-icon>mdi-login</v-icon>
					</v-list-item-icon>
					<v-list-item-content>
						<v-list-item-title>GraphQL Add Product</v-list-item-title>
					</v-list-item-content>
				</v-list-item>
			</router-link>
		<v-spacer></v-spacer>
	</v-app-bar>

	<v-content>
		<router-view/>
	</v-content>
</v-app>
</template>

<script>

export default {
	name: 'App',

	components: {
		//
	},

	data: () => ({
		//
	}),
};
</script>

<style scoped>
	.routerLink {
		text-decoration: none !important;
	}
</style>
