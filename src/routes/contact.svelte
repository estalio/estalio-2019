<svelte:head>
	<title>Contact Us</title>
</svelte:head>

<h1>Contact Us</h1>

<figure>
	<img alt='Contact Us' src='contact.png'>
</figure>

<p>Still have questions? Contact us and we will be happy to answer you.</p>

<form action="https://formspree.io/info@estalio.com" method="POST">
	<input type="text" name="name">
	<input type="text" name="email">
	<input type="text" name="subject">
	<textarea name="message" />
	<button type="submit">Send</button>
</form>
