<script lang="ts">
	import { Button } from "$lib/components/ui/button/index.js";
	import * as Card from "$lib/components/ui/card/index.js";
	import { Input } from "$lib/components/ui/input/index.js";
	import { Label } from "$lib/components/ui/label/index.js";
</script>

<Card.Root class="mx-auto max-w-sm">
	<Card.Header>
		<Card.Title class="text-2xl">Sign Up</Card.Title>
		<Card.Description>Join us today and unlock amazing features! Just enter your  email, username, and password to sign up</Card.Description>
	</Card.Header>
	<Card.Content>
		<div class="grid gap-4">
			<div class="grid gap-2">
				<Label for="email">Email</Label>
				<Input id="email" type="email" placeholder="user@example.com" required />
			</div>
			<div class="grid gap-2">
				<Label for="username">Username</Label>
				<Input id="username" type="input" placeholder="user" required />
			</div>
			<div class="grid gap-2">
				<div class="flex items-center">
					<Label for="password">Password</Label>
					<a href="##" class="ml-auto inline-block text-sm underline">
						Forgot your password?
					</a>
				</div>
				<Input id="password" type="password" required />
			</div>
			<Button type="submit" class="w-full">Sign Up</Button>
		</div>
		<div class="mt-4 text-center text-sm">
			Already have an account
			<a href="login" class="underline"> Sign in </a>
		</div>
	</Card.Content>
</Card.Root>
