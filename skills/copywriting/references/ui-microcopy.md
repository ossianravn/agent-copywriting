# Text inside a product

The reader is in the middle of a task and glances at the words on the way to the next action. Before writing, establish what they just did, what they see on the screen and what they want to do next. Read the product's existing strings and reuse its vocabulary.

Ask first whether the place needs text at all. A clear label, a sensible default or a visible state change often does the job, and a sentence that describes how the interface works is a sign that the interface should change. Tell the user when that is the case.

- **Buttons.** Name the outcome with a verb and, where needed, its object: "Save changes", "Delete project". An action has the same name everywhere it appears.
- **Labels.** Use the noun the reader would use for the thing.
- **Errors.** Say what happened in the reader's terms, then what they can do now. Place the message where the problem is.
- **Empty states.** Say what will appear here and offer the one action that makes it appear.
- **Confirmations of destructive actions.** Name the thing and the consequence. The button repeats the verb: "Delete 3 files".
- **Success.** Let the change on the screen confirm it where it can. Otherwise say briefly what happened.
- **Help text.** Give the one fact the reader needs to fill in the field correctly, such as a format or a limit.

Keep one term per concept across the whole product. Keep the tone calm and plain: the reader will see the same string many times.

Follow the conventions of the language and the platform for capitalisation, punctuation and forms of address. Write each string as a complete unit with placeholders for values, so that it can be translated and still read correctly with one item, several items and long words.

## Delivery

Return the strings in a table, so that a developer can place them:

| Where | Text | Shown when |
| --- | --- | --- |
| Upload dialog, error under the file field | The file is larger than 10 MB. Choose a smaller file. | The selected file exceeds the limit |
| Projects page, empty state | Your projects appear here. [Create project] | The account has no projects |
| Delete dialog, primary button | Delete project | Always |

For a cold read, give the reader the table and one line saying what the user was doing when the text appears.
