<script>
    export let data
</script>
<!-- Dashboard-info: info about dashboard -->
<section>
    <p>{data.infotext.markdown}</p>
</section>

<style>
    section {
        grid-area: dashboard-info;
        border-radius: .5rem;
        padding: 1.5rem;
        background-color: var(--whiteColor);
        box-shadow: var(--boxShadow) 0px 0px 8px;
        transition: .2s;
    }
    /* p {
		font-size: 1.3rem;
		line-height: 1.4;
	} */
     /*Section border gradient and animation*/
	section {
		position: relative;
	}
	section::after {
		--borderWidth: 3px;	
        content: '';
		position: absolute;
		top: calc(-1 * var(--borderWidth));
		left: calc(-1 * var(--borderWidth));
		height: calc(100% + var(--borderWidth) * 2);
		width: calc(100% + var(--borderWidth) * 2);
		background: linear-gradient(60deg, #f79533, #f37055, #ef4e7b, #a166ab, #5073b8, #1098ad, #07b39b, #6fba82);
  		border-radius: calc(2 * var(--borderWidth));
		z-index: -1;
		animation: gradient 3s ease alternate infinite;
		background-size: 400%;
	}

	@keyframes gradient {
		0% {
			background-position: 0% 50%;
		}
		50% {
			background-position: 100% 50%;
		}
		100% {
			background-position: 0% 50%;
		}
	}
</style>