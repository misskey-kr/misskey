<template>
<div>
	<div :class="$style.label" @click="focus"><slot name="label"></slot></div>
	<div :class="$style.content">
		<slot></slot>
	</div>
	<div :class="$style.caption"><slot name="caption"></slot></div>
</div>
</template>

<script lang="ts" setup>
import { } from 'vue';

function focus() {
	// TODO
}
</script>

<style lang="scss" module>
.label {
	font-size: 0.85em;
	padding: 0 0 8px 0;
	user-select: none;

	&:empty {
		display: none;
	}
}

.caption {
	font-size: 0.85em;
	padding: 8px 0 0 0;
	color: var(--fgTransparentWeak);

	&:empty {
		display: none;
	}
}
</style>
