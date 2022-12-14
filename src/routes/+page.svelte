<script>
	import { base } from '$app/paths';
	import data from '../data.js';
</script>

<svelte:head>
	<title>{data.seoTitle}</title>
	<meta name="description" content={data.seoDescription} />
	<link rel="preconnect" href="https://fonts.googleapis.com" />
	<link rel="preconnect" href="https://fonts.gstatic.com" crossorigin />
	<link
		href={`https://fonts.googleapis.com/css2?family=${data.font.replaceAll(' ', '+')}&display=swap`}
		rel="stylesheet"
	/>
</svelte:head>

<main style={`font-family: '${data.font}', sans-serif; color: ${data.fontColor}`}>
	<div class="section left-section">
		<header>
			<div style={`flex-grow: 1;`}>
				<img src="{base}/logo.png" alt="Mike Dane - Voice Talent" style="width: 15rem" />
				<!-- <h1 id="heading">{data.heading}</h1>
				<h2 id="sub-heading">{data.subheading}</h2> -->
			</div>
			<!-- <div id="microphone-icon">
				<svg
					xmlns="http://www.w3.org/2000/svg"
					xmlns:xlink="http://www.w3.org/1999/xlink"
					version="1.1"
					width="100%"
					height="100%"
					viewBox="0 0 256 256"
					xml:space="preserve"
				>
					<g
						style="stroke: none; stroke-width: 0; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: none; fill-rule: nonzero; opacity: 1;"
						transform="translate(1.4065934065934016 1.4065934065934016) scale(2.81 2.81)"
					>
						<path
							d="M 45 70.968 c -16.013 0 -29.042 -13.028 -29.042 -29.042 c 0 -1.712 1.388 -3.099 3.099 -3.099 c 1.712 0 3.099 1.388 3.099 3.099 C 22.157 54.522 32.404 64.77 45 64.77 c 12.595 0 22.843 -10.248 22.843 -22.843 c 0 -1.712 1.387 -3.099 3.099 -3.099 s 3.099 1.388 3.099 3.099 C 74.042 57.94 61.013 70.968 45 70.968 z"
							style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;"
							transform=" matrix(1 0 0 1 0 0) "
							stroke-linecap="round"
						/>
						<path
							d="M 45 60.738 L 45 60.738 c -10.285 0 -18.7 -8.415 -18.7 -18.7 V 18.7 C 26.3 8.415 34.715 0 45 0 h 0 c 10.285 0 18.7 8.415 18.7 18.7 v 23.337 C 63.7 52.322 55.285 60.738 45 60.738 z"
							style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;"
							transform=" matrix(1 0 0 1 0 0) "
							stroke-linecap="round"
						/>
						<path
							d="M 45 89.213 c -1.712 0 -3.099 -1.387 -3.099 -3.099 V 68.655 c 0 -1.712 1.388 -3.099 3.099 -3.099 c 1.712 0 3.099 1.387 3.099 3.099 v 17.459 C 48.099 87.826 46.712 89.213 45 89.213 z"
							style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;"
							transform=" matrix(1 0 0 1 0 0) "
							stroke-linecap="round"
						/>
						<path
							d="M 55.451 90 H 34.549 c -1.712 0 -3.099 -1.387 -3.099 -3.099 s 1.388 -3.099 3.099 -3.099 h 20.901 c 1.712 0 3.099 1.387 3.099 3.099 S 57.163 90 55.451 90 z"
							style="stroke: none; stroke-width: 1; stroke-dasharray: none; stroke-linecap: butt; stroke-linejoin: miter; stroke-miterlimit: 10; fill: rgb(0,0,0); fill-rule: nonzero; opacity: 1;"
							transform=" matrix(1 0 0 1 0 0) "
							stroke-linecap="round"
						/>
					</g>
				</svg>
			</div> -->
		</header>

		<div id="description">
			{#each data.description.split('\n') as p}
				<p>{p}</p>
			{/each}
			<div style="display: flex; align-items: center">
				<a
					id="contact-btn"
					style={`background: ${data.primaryColor}; color: ${data.fontColor}; box-shadow: 3px 3px 0px ${data.fontColor}`}
					href={`mailto: ${data.contactEmail}`}>Contact Me</a
				>
				<div style:font-weight="bold">{data.contactEmail}</div>
			</div>
		</div>
	</div>
	<div class="section right-section">
		<iframe
			style={`box-shadow: 5px 5px 0px ${data.fontColor};`}
			class="soundcloud"
			width="100%"
			height="400px"
			scrolling="no"
			frameborder="no"
			allow="autoplay"
			src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/playlists/1327235779&color=%23ff5500&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"
		/>
	</div>
	<div class="wave">
		<svg
			class="wave-svg"
			height="100%"
			viewBox="0 0 177 1343"
			fill="none"
			xmlns="http://www.w3.org/2000/svg"
		>
			<path
				d="M53.0736 713C164.674 401 99.5736 108.333 53.0736 1H176.07V1342H95.5736C34.9069 1262.33 -58.5264 1025 53.0736 713Z"
				fill={data.primaryColor}
			/>
		</svg>
		<div class="wave-body" style:background={data.primaryColor} />
	</div>
</main>

<style>
	#description {
		padding: 5px;
		padding-bottom: 10px;
		border-radius: 5px;
		background: white;
	}
	#contact-btn {
		width: 110px;
		text-decoration: none;
		height: 2rem;
		border-radius: 1rem;
		display: flex;
		justify-content: center;
		align-items: center;
		flex-shrink: 1;
		font-weight: bold;
		margin-right: 10px;
	}
	header {
		display: flex;
		flex-wrap: wrap;
		align-items: center;
	}
	#heading {
		font-size: 50px;
		margin: 0px;
	}
	#sub-heading {
		margin: 0px;
		font-size: 24px;
	}
	main {
		width: 100vw;
		min-height: 100vh;
		display: flex;
		alignitems: center;
		justify-content: space-around;
		flex-wrap: wrap;
	}
	@keyframes animate-pop {
		0% {
			opacity: 0;
			transform: translate(0px, -35px);
		}

		100% {
			opacity: 1;
			transform: scale(1, 1);
		}
	}
	.section {
		margin: 40px;
		display: flex;
		justify-content: center;
		flex-direction: column;
		animation-duration: 0.5s;
		animation-name: animate-pop;
		animation-timing-function: cubic-bezier(0.26, 0.53, 0.74, 1.48);
	}
	.left-section {
		flex-grow: 1;
		flex-shrink: 1;
		flex-basis: 300px;
		max-width: 500px;
	}
	.right-section {
		flex-grow: 1;
		flex-shrink: 1;
		flex-basis: 300px;
		min-width: 350px;
		max-width: 750px;
		width: 750px;
	}
	.soundcloud {
		border-radius: 3px;
	}
	.wave {
		position: absolute;
		right: 0px;
		z-index: -1;
		width: 50%;
		height: 100%;
		display: flex;
	}
	.wave-svg {
		margin-right: -1px;
	}
	.wave-body {
		flex-grow: 1;
		background: #2acdb0;
	}
	#microphone-icon {
		width: 50px;
		height: 50px;
		margin: 10px;
	}
</style>
