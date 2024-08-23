<h4>Analytic Rules</h4>
<p>detecting suspicious activities and potential threats. Creating these rules collected by Sentinel, looking for patterns. When a rule identifies a threat, it triggers an alert, allowing security teams to investigate and respond quickly.  </p>
<p>
  <img src="https://github.com/user-attachments/assets/f8ef10ef-4cd2-49a1-8f9d-df2efa4e66ae" height="80%" width="80%" />
</p>
<p>
I created an Analytic Rule called TEST: BRUTE FORCE to identify threats if someone is attempting to log into the same VM 10 times in the last 60mins. </p>

  <p>
  <img src="https://github.com/user-attachments/assets/24a365d1-6886-419f-8345-5066fad9470a" height="80%" width="80%" />
    <p>I used a query for failed login attempts using EventID 4625. it then counts how many times each IP address(AtackerIP) has failed to log in. As you can see, we have over 10 failed logins. </p>
  </p>
<p>
   <img src="https://github.com/user-attachments/assets/defb6aa7-18d2-4eb1-9610-44c1c19372a8" height="80%" width="80%" />
</p>
<p>The Severity is set to Medium which means that the alert is significant and should be addressed very soon but might not be as urgent as a High Severity alert. Sometimes it could mean potential malicious activity that could be a risk if it's not investigated
immediately.</p>
 
