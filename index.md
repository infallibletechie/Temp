<html>
  Email Id is <p id="emailStr"></p>
  <script>
    const params = new URLSearchParams(
      window.location.search
    );
    console.log(
      'params are',
      params.toString()
    );
    let strEmailId = 
        params.has( 'emailId' ) ?
        params.get( 'emailId' ) : 
        'Email Id not passed';
    console.log(
        'Email Id is',
        strEmailId.replace( 
    		' ', 
    		'+' 
    	)
    );
    document.getElementById( 'emailStr' ).innerHTML = strEmailId.toString();
  </script>
</html>
