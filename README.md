

<h2>Google Geocoding API Automated Test Exercise</h2>

<h3>Description:</h3>

This is a brief automated test that validates that the Google Geocoding API is functioning correctly. It uses Postman (an API development and testing tool) to accomplish this.


<h3>Getting Started:</h3>

The following instructions provide you with the details you need in order to get copy of the test suite running on your local machine.

<ul>
<li><a href="https://docs.google.com/document/d/e/2PACX-1vTrZtog6zc40Xo2j5mSHJXpLbA5B6MFVFxRfIj5MwLzieY-J6ceSwtUXZrSFXGcku41JDs1L0c094yc/pub">Test Plan</a></li>


<li><a href="https://docs.google.com/spreadsheets/d/e/2PACX-1vQ0yJPKghz6r3dE4V_opcBYlL904Xfk9CQC-AWD71zPR9cV_JmBlw_MKNzExRHDnYt3x-TPiSGkzC3A/pubhtml">Test Steps</a></li>

</ul>

<h3><u>Test Data:</u></h3>

Google App API Key: For security purposes this has been added to <a href="https://www.lastpass.com/">LastPass</a>.  Please contact administrator for access.


<u><h3>Test Setup:</h3></u>

1. Download the <a href="https://www.getpostman.com/apps">Postman</a> application.


2. Enable your <a href="https://developers.google.com/maps/documentation/geocoding/get-api-key">Google Geocoding API Key</a> 

3. Enable the Geocoding API in your Google Cloud platform for your project. <br>
<b>Note:</b> If the API is not enabled an error will be returned when attempting to send a request.


	A. Navigate to your Google Cloud Platform <br>
	B. Select Google maps in the right navigation menu <br>
	C. Select APIs in the Google maps right navigation menu <br>
	D. Select Geocoding API under In use APIs <br>
	E. Click Enable

4. Attempt to send a request and verify that it is successful (200 response).

5. Follow the <a href="http://blog.getpostman.com/2014/03/07/writing-automated-tests-for-apis-using-postman/">Postman automated test documentation.</a>

6. Add API key to your Geocoding request.<br>
http://maps.googleapis.com/maps/api/geocode/json?address=49+bogart+St,+San+brooklyn,+Ny&key='YOUR_API_KEY'

7. Add API key to your Geocoding reverse request.<br>
https://maps.googleapis.com/maps/api/geocode/json?latlng=40.7053762,-73.9335617&&key='YOUR_API_KEY'

8. Use the provided <a href="https://github.com/rharley77/Consensys-API-Automation-Exercise/tree/master/Postman%20Test%20Files"> Javascript Test Files</a> for Postman test execution.

9. Kick off an automated test with the Postman Collection Runner. <br>
<b>Note:</b> The Consensys Exercise.postman_test_run.json file includes test run results and can be uploaded to the Postman Collection Runner. This requires you to update the You API Key with an active API key.
<ul>
<li>Test run results example <a href="https://screencast.com/t/i9nFSpJGA">video</a></li>
</ul>

10. Once stabilized add the automated test suite to your CI integration test build. They should be included in the tests that are run with every Pull Request that is opened.

