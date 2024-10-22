<script>

</script>


<svelte:head>
	<title>Contact Me</title>
	<meta name="description" content="Contact Me" />
</svelte:head>

<br />

<h1>Contact Me</h1>
<div class="container">

   <div class="socials"> 
	<div class="call">
		<h2>Call</h2>
	<a href="tel:+25147340602" class="socials">
		<svg xmlns="http://www.w3.org/2000/svg" width="60" height="60" viewBox="0 0 24 24" {...$$props}>
			<path fill="currentColor" fill-opacity="0" stroke="currentColor" stroke-dasharray="64" stroke-dashoffset="64" stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 3c0.5 0 2.5 4.5 2.5 5c0 1 -1.5 2 -2 3c-0.5 1 0.5 2 1.5 3c0.39 0.39 2 2 3 1.5c1 -0.5 2 -2 3 -2c0.5 0 5 2 5 2.5c0 2 -1.5 3.5 -3 4c-1.5 0.5 -2.5 0.5 -4.5 0c-2 -0.5 -3.5 -1 -6 -3.5c-2.5 -2.5 -3 -4 -3.5 -6c-0.5 -2 -0.5 -3 0 -4.5c0.5 -1.5 2 -3 4 -3Z">
				<animate fill="freeze" attributeName="fill-opacity" begin="0.7s" dur="0.5s" values="0;1" />
				<animate fill="freeze" attributeName="stroke-dashoffset" dur="0.6s" values="64;0" />
			</path>
		</svg>	
	</a>
	</div>

	<div class="email">
		<h2>Email</h2>
		<a href="mailto:nahusenaytadesse75@gmail.com" target="_blank"> 
			<svg xmlns="http://www.w3.org/2000/svg" width="30" height="40" viewBox="0 0 24 24" {...$$props}>
				<path fill="currentColor" d="m20 8l-8 5l-8-5V6l8 5l8-5m0-2H4c-1.11 0-2 .89-2 2v12a2 2 0 0 0 2 2h16a2 2 0 0 0 2-2V6a2 2 0 0 0-2-2" />
			</svg>		 
		</a>
		</div>
   </div>
<form action="contact">
	<label for="">Name</label>
	<input type="text" placeholder="Name">
	<label for="">Phone Number</label>
	<input type="tel" placeholder="Phone Number" name="" id="phone">
	<label for="">Email</label>
	<input type="email" name="" id="" placeholder="Email">
	<label for="">Messages</label>
	<input type="text" name="" id="message" placeholder="Message">
	<input type="submit" value="Submit" id="submit">

</form>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		justify-content: space-around;
		align-items: center;
		height: 70vh;
	}
	@media (max-width: 768px) {
		.container {
			flex-direction: column;
			width: 100%;
		}
		
		form {
			width: 400px;
			align-items: center;
		}
		input {
			width: 300px;
		}
		#submit {
			width: 300px;
		}
	}
	.socials {
		 display: flex;
		 flex-direction: row;
		 justify-content: space-evenly;
		 align-items: start;
		 width: 50%;
	}
	form {
		display: flex;
		flex-direction: column;
		width: 60%;
		align-self: center;
		justify-content: space-around;
		gap: 10px;
	}
	#message {
		padding-bottom: 10%;
	}
	input {
		margin-bottom: 10px;
		border: none;
		font-size: 20px;
		height: 22px;
		padding-bottom: 10px;
	}
	label {
		font-size: 16px;
		display: none;
	}
	input::placeholder {
		font-size: 12px;
	}

	input:focus {
		background-color: #fefefe;
		border: none;
		font-size: 12px;
	}
	
	#submit{
		background-color: var(--color-theme-1);
        color: white;
        text-decoration: none;	
        width: 100%;
        padding: 10px;
        border: solid 1px;
        text-align: center;
        border-radius: 8px;
		height: 40px;
		font-size: 16px;
	}
	#submit:hover {
		background-color: transparent;
		color: var(--background)
	}
	
	#message:focus {
	    border: 30px;
	}
	svg:hover {
		color: var(--color-theme-2);
	}
    .email h2{
      margin-bottom: 20px;
	}
</style>