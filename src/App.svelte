<script>
  import Email from "@nylas/components-email";
  const staticThread = {
    account_id: "account-id-0",
    drafts: [],
    first_message_timestamp: 1626822389,
    has_attachments: false,
    id: "thread-id",
    folders: [
      {
        display_name: "Important",
        id: "folder-id",
        name: "important"
      }
    ],
    last_message_received_timestamp: 1626822389,
    last_message_sent_timestamp: 1626822419,
    last_message_timestamp: 1626822419,
    messages: [
      {
        account_id: "account-id-1",
        bcc: [],
        cc: [
          {
            email: "al@particletech.com",
            name: "Albert Einstein"
          }
        ],
        body:
          "Hello folks! The idea is coming together soon. It will actually be my brightest idea <strong>ever</strong>.",
        date: 1626822419,
        files: [],
        from: [
          {
            email: "tom@brightideas.com",
            name: "Thomas Edison"
          }
        ],
        id: "message-id-0",
        labels: [
          {
            display_name: "Inbox",
            id: "label-id-0",
            name: "inbox"
          }
        ],
        object: "message",
        reply_to: [
          {
            email: "tom@brightideas.com",
            name: "Thomas Edison"
          }
        ],
        snippet: "Hello folks! The idea is coming together soon.",
        starred: false,
        subject: "Re: Tom's Brightest Idea",
        thread_id: "thread-id-0",
        to: [
          {
            email: "alex@bell.com",
            name: "Alexander Graham Bell"
          },
          {
            email: "marie@radioactivity.com",
            name: "Marie Curie"
          }
        ],
        unread: true
      },
      {
        account_id: "account-id-2",
        bcc: [],
        cc: [],
        body:
          "Tom seems to be cooking up something... We just got off the phone and he sounded very excited, let's see what he says",
        date: 1626822389,
        files: [],
        from: [
          {
            email: "marie@radioactivity.com",
            name: "Marie Curie"
          }
        ],
        id: "message-id-1",
        labels: [
          {
            display_name: "Inbox",
            id: "label-id-0",
            name: "inbox"
          }
        ],
        object: "message",
        reply_to: [
          {
            email: "marie@radioactivity.com",
            name: "Marie Curie"
          }
        ],
        snippet: "Tom seems to be cooking up something...",
        starred: true,
        subject: "Tom's Brightest Idea",
        thread_id: "thread-id-0",
        to: [
          {
            email: "alex@bell.com",
            name: "Alexander Graham Bell"
          },
          {
            email: "tom@brightideas.com",
            name: "Thomas Edison"
          }
        ],
        unread: false
      }
    ],
    object: "thread",
    participants: [
      {
        email: "tom@brightideas.com",
        name: "Thomas Edison"
      },
      {
        email: "alex@bell.com",
        name: "Alexander Graham Bell"
      },
      {
        email: "marie@radioactivity.com",
        name: "Marie Curie"
      },
      {
        email: "al@particletech.com",
        name: "Albert Einstein"
      }
    ],
    snippet: "Tom seems to be cooking up something...",
    starred: true,
    subject: "Tom's Brightest Idea",
    unread: true,
    version: 1
  };
</script>

<style>
  main {
    font-family: sans-serif;
  }
  iframe {
    display: none;
  }
</style>

<main>
    <h1>Nylas Email</h1>
    <h2>Passing in a thread</h2>
    <nylas-email thread={staticThread}/>
    <h2>Passing in a single message</h2>
    <nylas-email message={staticThread.messages[0]}/>
</main>