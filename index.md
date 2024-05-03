<html>
	<script>
		function playAudio() {
			
			console.log(
				'Inside playAudio'
			);
			let objSound = document.getElementById("AudioId");
			objSound.play();
			console.log(
				'playAudio End'
			);
		
		}
	</script>
    <audio id="AudioId">
        <source 
			src="https://infallibletechie2-dev-ed--c.develop.vf.force.com/resource/1714752960000/SampleMusic" 
			type="audio/mpeg">
    </audio>	
	<button onclick="playAudio()">
		Play Audio
	</button>
</html>
