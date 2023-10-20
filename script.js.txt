document.addEventListener("DOMContentLoaded", function () {
    const affirmationButton = document.getElementById("showAffirmation");
    const affirmationPopup = document.getElementById("affirmationPopup");
    const affirmationText = document.getElementById("affirmationText");
    const closePopupButton = document.getElementById("closePopup");

    // Define an array of daily affirmations
    const affirmations = [
        "I am confident and capable.",
        "I attract positivity into my life.",
        "I am deserving of love and happiness.",
        "I am capable of achieving anything I set my mind to",
        "It is okay to need rest",
        "pay attention to who you are with when you feel your best.",
        "make yourself a priority.",
        "I know these feelings that drain me are temporary.",
        "Mom, I am a rich man- Cher.",
        "I was not born to be subtle.",
        "I will turn this anger into something beautiful.",
        "What is mine will not pass by me.",
        "God does not burden any soul with more than it can bear",
        
    
        // Add more affirmations here
    ];

    affirmationButton.addEventListener("click", function () {
        // Select a random affirmation from the array
        const randomIndex = Math.floor(Math.random() * affirmations.length);
        const selectedAffirmation = affirmations[randomIndex];

        // Display the selected affirmation in the popup
        affirmationText.textContent = selectedAffirmation;

        // Show the popup
        affirmationPopup.style.display = "block";
    });

    closePopupButton.addEventListener("click", function () {
        // Close the popup
        affirmationPopup.style.display = "none";
    });
});
