(function() {
    // List of funny sounds to play
    var sounds = [
        "https://s3.amazonaws.com/freecodecamp/simonSound1.mp3",
        "https://s3.amazonaws.com/freecodecamp/simonSound2.mp3",
        "https://s3.amazonaws.com/freecodecamp/simonSound3.mp3",
        "https://s3.amazonaws.com/freecodecamp/simonSound4.mp3"
    ];

    // Choose a random sound to play
    var soundToPlay = sounds[Math.floor(Math.random() * sounds.length)];

    // Play the chosen sound
    var audio = new Audio(soundToPlay);
    audio.play();

    // Get all elements in the document
    var allElements = document.getElementsByTagName('*');

    // Iterate through each element and change its font size randomly
    for (var i = 0; i < allElements.length; i++) {
        allElements[i].style.fontSize = Math.floor(Math.random() * 30) + "px";
    }

    // Create a prank alert to be shown to the user
    var prankAlert = alert("
