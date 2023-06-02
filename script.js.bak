$(document).ready(function() {
    $('form').submit(function(e) {
        e.preventDefault(); // Prevent the form from submitting normally

        // Perform an AJAX request to the send_email.php file
        $.ajax({
            type: 'POST',
            url: $(this).attr('action'),
            data: $(this).serialize(),
            success: function(response) {
                // Display the response message
                alert(response);
                // You can also update the UI to show the response message in a specific element on the page
            },
            error: function() {
                alert('An error occurred while sending the message.');
            }
        });
    });
});
