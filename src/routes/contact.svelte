<style>
	.form-input {
		margin: 0px auto;
	}

	input, textarea {
		width: 75%;
	}
</style>

<svelte:head>
	<title>Contact Us - Estalio Consulting Inc.</title>
</svelte:head>

<h1>Contact Us</h1>

<figure>
	<img alt='Contact Us' src='contact.png'>
</figure>

<p>Still have questions? Contact us and we will be happy to answer you.</p>

<form action="https://formspree.io/info@estalio.com" method="POST">
	<div class="form-input">
		<input type="text" name="name">
	</div>
	<div class="form-input">
		<input type="text" name="email">
	</div>
	<div class="form-input">
		<input type="text" name="subject">
	</div>
	<div class="form-input">
		<textarea name="message" />
	</div>
	<div class="form-input">
		<button type="submit">Send</button>
	</div>
</form>
