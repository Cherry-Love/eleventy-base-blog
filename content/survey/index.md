---
layout: layouts/base.njk
eleventyNavigation:
  key: Survey
  order: 5
---
# Survey

<form id="survey-from" name="survey-from" method="POST" netlify>
  <fieldset>
	<div class="mb-3">
		<label for="survey-title" class="form-label">Title</label>
		<select class="form-select" aria-label="Choose the title" id="survey-name-title" name="survey-name-title">
			<option value="" selected>--Choose the title--</option>
			<option value="Mr">Mr.</option>
			<option value="Miss">Miss</option>
			<option value="Ms.">Ms.</option>
			<option value="Mrs.">Mrs.</option>
			<option value="Mx.">Mx.</option>
		</select>
		</div>
		<div class="mb-3">
			<label for="survey-Name" class="form-label">Choose your Nickname*</label>
			<input type="text" class="form-control" id="survey-Name" name="survey-Name" placeholder="Your name" required>
		</div>
		<div class="mb-3">
			<label for="survey-avatar" class="form-label">Choose your avatar (png, jpg, jpeg, less than 1MB)</label>
			<input class="form-control" type="file" id="survey-avatar" name="survey-avatar">
		</div>
		<div class="mb-3">
		 <label for="gender" class="form-label">Your gender:</label>
      <select id="gender" name="gender" disabled  class="form-select" aria-label="Choose the gender" >
        <option value="" selected>--Choose the gender--</option>
				<option value="male">Male</option>
        <option value="female">Female</option>
        <option value="other">Prefer not to say</option>
      </select>
		</div>
		<div class="mb-3">
			<label for="survey-DOB" class="form-label" >Date of Birth</label>
			<input type="date" class="form-control" id="survey-DOB" name="survey-DOB" min="1940-01-01" max="2013-01-01">
		</div>
		<div class="mb-3">
			<label for="survey-email" class="form-label">Email address*</label>
			<input type="email" class="form-control" id="survey-email" name="survey-email" aria-describedby="emailHelp" placeholder="name@example.com" required>
			<div id="emailHelp" class="form-text">We'll never share your email with anyone else.</div>
		</div>
  </fieldset>
	<fieldset id="hobbies">
		<div class="mb-3">
			<label for="survey-hobbie" class="form-label">Your hobby</label>
			<input type="text" class="form-control" id="survey-hobbie" name="survey-hobbie" placeholder="Knitting, painting, etc.">
		</div>
		<div class="mb-3">
			<label for="survey-favBook" class="form-label">Your favorite book</label>
			<input type="text" class="form-control" id="survey-favBook" name="survey-favBook" placeholder="Book name, author...">
		</div>
		<div class="mb-3">
			<label for="survey-favMovie" class="form-label">Your favorite movie</label>
			<input type="text" class="form-control" id="survey-favMovie" name="survey-favMovie" placeholder="Movie name, year...">
		</div>
	</fieldset>
	<fieldset id="employ-status">
		<div class="mb-3">
			<label class="form-check-label" for="time-spent">Your current employment status</label>
		</div>
		<div class="form-check">
			<input class="form-check-input" type="radio" name="employmentStat" id="empoyed">
			<label class="form-check-label" for="empoyed">Empoyed</label>
		</div>
			<div class="form-check">
			<input class="form-check-input" type="radio" name="employmentStat" id="unempoyed">
			<label class="form-check-label" for="unempoyed">Unempoyed</label>
		</div>
			<div class="form-check">
			<input class="form-check-input" type="radio" name="employmentStat" id="student">
			<label class="form-check-label" for="student">Student</label>
		</div>
			<div class="form-check">
			<input class="form-check-input" type="radio" name="employmentStat" id="retired">
			<label class="form-check-label" for="retired">Retired</label>
		</div>
	</fieldset>
	<fieldset id="time-spent">
		<div class="mb-3">
			<label class="form-check-label" for="time-spent">What do you spent your free time on?</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="movies" name="time-spenting">
			<label class="form-check-label" for="movies">Watching movies, tv shows</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="books" name="time-spenting">
			<label class="form-check-label" for="books">Reading books</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="shopping" name="time-spenting">
			<label class="form-check-label" for="shopping">Make shopping</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="social-media" name="time-spenting">
			<label class="form-check-label" for="social-media">Social media (Facebook, Twitter, TikTok, etc.)</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="learning" name="time-spenting">
			<label class="form-check-label" for="learning">Learning something new</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="active-rest" name="time-spenting">
			<label class="form-check-label" for="active-rest">Active rest (Climbing mountains, boating, camping, etc.)</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="music" name="time-spenting">
			<label class="form-check-label" for="music">Listening music</label>
		</div>
		<div class="mb-3 form-check">
			<input type="checkbox" class="form-check-input" id="relax" name="time-spenting">
			<label class="form-check-label" for="relax">Relaxing, meditation or even sleeping</label>
		</div>
	</fieldset>
  <div class="mb-3 form-check">
    <input type="checkbox" class="form-check-input" id="exampleCheck1" disabled checked>
    <label class="form-check-label" for="exampleCheck1" >By clicking "Submit" button you agree that information being shared and gathered between services</label>
  </div>



  <input type="submit" class="btn btn-primary" id="submit">
</form>
