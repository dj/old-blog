+++
date = "2017-08-27T00:00:00-00:00"
draft = false
title = "Contact"

+++

<form name="contact" action="thank-you" netlify>
	<fielset>
		<label>Your Name: <input type="text" name="name"></label>   
	</fielset>
	<fielset>
		<label>Your Email: <input type="email" name="email"></label>
	</fielset>
	<fielset>
		<label>Message: <textarea name="message"></textarea></label>
	</fielset>
    <button type="submit">Submit</button>
</form>

<style>
	fielset, input, textarea {
		width: 100%;
		display: block;
	}
</style>
