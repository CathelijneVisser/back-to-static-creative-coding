<script>
    export let data
    export let text
</script>

<section class="box-1">
    <h2>{new Intl.NumberFormat().format(data.debris_extracted_total)} KG</h2>
    <p>{text.dashboard.trashRemoved.total}</p>
</section>

<section class="box-2">
    <h2>{new Intl.NumberFormat().format(data.debris_extracted_last_30d)} KG</h2>
    <p>{text.dashboard.trashRemoved.month}</p>
</section>

<style>
    section {
        border-radius: .5rem;
        padding: 1.5rem;
        background-color: var(--trashRemovedBackground);
        box-shadow: var(--boxShadow) 0px 0px 8px;
        transition: .2s;
        /* border: 20px solid var(--lightBlue) */
    }
    .box-1 {
        grid-area: box-1;
    }

    .box-2 {
        grid-area: box-2;
    }

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
		background: linear-gradient(60deg, #dd3e54, #6be585);
  		border-radius: calc(2 * var(--borderWidth));
		z-index: -1;
		animation: gradient 6s ease alternate infinite;
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