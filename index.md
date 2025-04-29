# First level headline

This is a test page with a [test file](example/test.xlsx). And another [test file](example/test.html).

## Second level headline

This example really needs some structure.

## Additional second level headline

And more content.

# Test page counter

<script>
        const namespace = 'pascalkieslichtest'; // Replace with your namespace
        const counterName = 'pascaltestcounter'; // Replace with your counter name
        const apiUrl = `https://api.counterapi.dev/v1/${namespace}/${counterName}/up`;

        // Increment the count
        fetch(apiUrl)
            .then(response => response.json())
            .then(data => {
                console.log('Page views:', data.count);
                document.body.insertAdjacentHTML('beforeend', `<p>This page has been viewed ${data.count} times.</p>`);
            })
            .catch(error => console.error('Error:', error));
</script>
