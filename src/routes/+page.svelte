<script lang="ts">
	import { Button } from '$lib/components/ui/button/index.js';
	import { Textarea } from '$lib/components/ui/textarea/index.js';
	import * as Select from '$lib/components/ui/select/index.js';
</script>

<div>
	<p>This is a simple Svelte component with a button.</p>

	<Textarea placeholder="Type your message here." />

	<Select.Root type="single">
		<Select.Trigger class="w-[180px]"></Select.Trigger>
		<Select.Content>
			<Select.Item value="light">Light</Select.Item>
			<Select.Item value="dark">Dark</Select.Item>
			<Select.Item value="system">System</Select.Item>
		</Select.Content>
	</Select.Root>

	<Button>Click Me</Button>
</div>

<style>
</style>
