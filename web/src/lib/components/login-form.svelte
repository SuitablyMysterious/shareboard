<script lang="ts">
	import { Button } from "$lib/components/ui/button/index.js";
	import * as Card from "$lib/components/ui/card/index.js";
	import { Input } from "$lib/components/ui/input/index.js";
	import {
		FieldGroup,
		Field,
		FieldLabel,
		FieldDescription,
	} from "$lib/components/ui/field/index.js";

	const id = $props.id();
</script>

<Card.Root class="mx-auto w-full max-w-sm">
	<Card.Header>
		<Card.Title class="text-2xl">Join Room</Card.Title>
		<Card.Description>Enter your room id</Card.Description>
	</Card.Header>
	<Card.Content>
		<form>
			<FieldGroup>
				<Field>
					<FieldLabel for="room-{id}">Room</FieldLabel>
					<Input id="room-{id}" type="string" placeholder="AbcD12" required />
				</Field>
			</FieldGroup>
		</form>
	</Card.Content>
</Card.Root>
