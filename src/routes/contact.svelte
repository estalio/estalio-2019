<style>
	h1 {
		font-size: 2.8em;
		text-transform: uppercase;
		font-weight: 700;
		margin: 0 0 0.5em 0;
	}

	figure {
		margin: 0 0 0 2em;
		float: right;
		width: 40vh;
	}

	img {
		width: 100%;
		max-width: 400px;
		margin: 0 0 1em 0;
	}

	p {
		margin: 1em auto;
		text-align: justify;
	}

	.form-input {
		margin: 1em auto;
	}

	form {
		float: left;
		width: 40%;
	}

	input, textarea {
		width: 100%;
		display: block;
	}

	textarea {
		height: 5em;
	}

	button {
		background-color: #555555;
		border: none;
		color: white;
		text-align: center;
		text-decoration: none;
		font-size: 16px;
		padding: 0.5em;
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

<form
  action="https://formspree.io/f/mjvjbnre"
  method="POST"
>
	<div class="form-input">
		<label for="name">Name</label>
		<input type="text" name="name" id="name" />
	</div>
	<div class="form-input">
		<label for="email">Email</label>
		<input type="email" name="email" id="email" />
	</div>
	<div class="form-input">
		<label for="subject">Subject</label>
		<input type="text" name="subject" id="subject" />
	</div>
	<div class="form-input">
		<label for="message">Message</label>
		<textarea name="message" id="message" />
	</div>
	<div class="form-input">
		<button type="submit">Send</button>
	</div>
</form>
