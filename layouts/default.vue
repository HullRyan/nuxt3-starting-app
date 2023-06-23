<template>
	<div class="flex flex-col h-screen">
		<navigation-bar />
        <div class="flex-grow">
            <slot />
        </div>
        <footer-bar />
	</div>
</template>
