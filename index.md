<html>
  Email Id is <p id="emailStr"></p>
  <script>
    const params = new URLSearchParams(
      window.location.search
    );
    console.log(
      'params are',
      JSON.stringify( params )
    );
    let varEmailId = 
        params.has( 'emailId' ) ?
        params.get( 'emailId' ) : 
        'Email Id not passed';
    console.log(
        'Email Id is',
        varEmailId
    );
    document.getElementById( 'emailStr' ).innerHTML = varEmailId;
  </script>
</html>
