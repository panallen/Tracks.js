Tracks.js
=========

A lightweight mutlitrack html media player.

    <audio>
        <source src="first_track.ogg" type="audio/ogg" />
        <source src="first_track.mp3" type="audio/mp3" />
    </audio>
    <audio>
        <source src="second_track.ogg" type="audio/ogg" />
        <source src="second_track.mp3" type="audio/mp3" />
    </audio>

    <script type="text/javascript">
        var song = new tracks.Tracks(document.getElementsByTagName('audio'));
        song.on('canplay', function(){
            this.play();
        });
    </script>