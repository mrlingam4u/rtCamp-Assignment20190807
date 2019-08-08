# rtCamp-Assignment20190807

//Test objective 1:
<?php
$I->amOnPage('/bp-login-form');
$I->fillField('Username', 'demo');
$I->fillField('Password', 'demo');
$I->click('Log In');
$I->see('Howdy, demo');


//Test objective 2:
<?php
$I->amOnPage('/bp-login-form');
$I->fillField('Username', 'demo1');
$I->fillField('Password', 'demo1');
$I->click('Log In');
$I->see('ERROR: Invalid username.');


//Test objective 3:
<form method="post" action="/update" id="update_form">
     <input type="text" id="whats-new" />
     <select id="rtSelectPrivacy">
          <option value="Private">Private</option>
          <option value="Loged in users">User</option>
          <option value="Public">Public</option>
     </select>
     <input type="submit" name="aw-whats-new-submit" value="Update" />
</form>


//Test objective 4:
<form method="post" action="/update" id="rtmedia-nav-item-albums">
  $I->click('Upload');
  <select id="rtSelectPrivacy">
          <option value="Private">Private</option>
          <option value="Loged in users">User</option>
          <option value="Public">Public</option>
     </select>
     <input type="submit" name="rtMedia-upload-button"/>
$I->click('Start upload')
</form>


//Test objective 4:
<form method="post" action="/update" id="rtmedia-like-counter-wrap">
  $I->click('Like');
  $I->click('You like this');
</form>



Test objective 5:
<form method="post" action="/update" id="change-cover-image">
  $I->click('Select your File');
</form>
