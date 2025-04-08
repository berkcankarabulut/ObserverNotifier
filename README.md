<h3> Notifier (Observer-Based Notification System)</h3>
    <p>Lightweight messaging system for <strong>independent component communication.</strong></p>
    <ul>
        <li><code>Subscribe(T handler)</code> → Adds an event listener.</li>
        <li><code>Unsubscribe(T handler)</code> → Removes an event listener.</li>
        <li><code>Notify(T data)</code> → Triggers an event.</li>
    </ul>
    <pre><code>Notifier<string> messageNotifier = new Notifier<string>();
messageNotifier.Subscribe(msg => Debug.Log("Received: " + msg));
messageNotifier.Notify("Hello, World!");
    </code></pre>
