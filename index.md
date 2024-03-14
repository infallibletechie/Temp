<html>
  <script>
    const params = new URLSearchParams(
      window.location.search
    );
    let varEmailId = 
        params.has( 'emailId' ) ?
        params.get( 'emailId' ) : 
        ''Email Id not passed';
    console.log(
        'Email Id is',
        varEmailId
    );
    document.getElementById( 'emailStr' ).innerHTML = varEmailId;
  </script>
  Email Id is <p id="emailStr"></p>
</html>
