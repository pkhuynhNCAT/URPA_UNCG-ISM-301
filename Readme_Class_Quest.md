# Class Quest — The Clinic Case

**A guided learning game for UNCG — ISM301: Systems and Process Analysis**  
Structural Modeling · Version 3.2

Welcome to Class Quest. You will help a small veterinary clinic work out what its software needs to remember. You will meet Bella the dog, create pet records, follow an appointment, and connect pets to their owners. Then you will use those ideas to choose classes and repair a class diagram.

**You do not need to know UML or programming before you start.** Pip, the little robot guide, explains each action. You can take your time, ask for hints, and try again. There is no timer, and a wrong answer never takes points away.

The two files are:

| File | What it is for |
|---|---|
| **Class_Quest.html** | The whole game. Download this file and open it in a browser. |
| **Readme.md** | This guide. It explains how to play, what you will learn, and how to keep your work. |

The app works on its own. It does not need this README, separate pictures, an account, or an internet connection.

**Find what you need:** [Start the game](#1-start-here) · [Learning path](#4-the-learning-path) · [Mission 1](#8-mission-1--find-the-classes) · [Mission 2](#9-mission-2--repair-the-diagram) · [Save your work](#12-keep-your-notes-and-progress) · [Common questions](#14-common-questions) · [Instructor notes](#16-notes-for-instructors)

## 1. Start here

1. **Download Class_Quest.html** to your computer.
2. Find it in your Downloads folder.
3. Open it in a web browser. If double-clicking opens a text editor, right-click the file and choose **Open with**, then your browser.
4. On the welcome screen, choose **Start with Pip**.
5. Look below the picture for Pip’s task card. Read the short instruction, then click its large green action button.
6. Watch what changes. Read **Here’s what changed** in the same task card.
7. Choose **I see it. Continue** when you are ready.

Keep using the same pattern: **read → try → notice → continue**.

At the end of each chapter, the task card asks one question. Its answer buttons sit directly under the question. Choose an answer, read the feedback, and try again if needed. The question, choices, hints, and explanation stay together below the picture.

If you have already played, the welcome button may say **Continue my guided adventure**, **Continue Mission 1**, or **Continue Mission 2**. The app uses your saved progress to suggest a next activity. Opening the same file can also take you straight back to the activity you left.

**If you feel lost at any time, choose How to play at the top.** It tells you where you are, what you are doing, and what to click next. Close it with **Back to my activity** to return to the same place.

> A Google Drive, email, or course-site preview may show the file without running the game. Download the HTML and open the downloaded copy in a browser. You do not need to install anything or run a command.

## 2. Your first few clicks, explained

Here is exactly how the opening works.

**First, meet Bella.** Pip explains that Bella is arriving at the clinic. Choose **Let Bella into the clinic**. Bella moves into the scene. Pip explains that the clinic needs to remember information about this particular dog.

**Next, make a template.** Choose **I see it. Continue**, then **Make the Pet template**. You will see a reusable Pet form. This is your first class.

**Add spaces for facts.** Continue again, then choose **Add spaces for the facts**. Name, species, and weight are examples of information that each pet record can hold. These spaces are called attributes.

**Make Bella’s record.** Continue and choose **Create Bella’s record**. A filled record appears. The template is still available, so you can use it again for Max.

You are learning through the changes you make. You do not need to memorize all the new words before trying the next action.

### When an instruction is unclear

- **I’m not sure** gives a simpler explanation.
- **Show me exactly** gives the most direct help, including the action or answer to choose.
- **Replay the motion** repeats a completed action so you can watch again.
- **Previous step** lets you revisit the last part.
- **Settings → Reduce motion** stops movement while keeping the completed scene and information visible.

At the end of a chapter, choose an answer to one short question. A wrong answer gives a clue. Try again and read the explanation. These opening checks are practice, and they do not change your XP.

## 3. What does this have to do with ISM301?

In Systems and Process Analysis, you learn to understand a business before building its software. This game practices Structural Modeling. You will discover what needs a record and how those records connect in the system.

In **Structural Modeling**, you represent those decisions using classes and relationships. A **UML class diagram** is a picture of those classes and their connections. UML is the name of the diagram language used in the course.

Class Quest gives you a small, concrete business to think about. After playing, you should be able to explain why Pet is a class, why Bella is an individual object, and why a cancelled appointment should not disappear. You should also be able to read the numbers on a relationship and notice when a diagram makes the wrong claim about the business.

The game gives you guided practice. It does not ask you to write code or draw a completely new diagram from a blank page. Your instructor can use a later exercise to help you build a model independently.

## 4. The learning path

| Part | What you do | What you learn |
|---|---|---|
| **Learn with Pip** | Follow 19 small steps in three animated chapters. | What classes, records, actions, and relationship numbers mean. |
| **Practice playground** | Repeat the examples and change their outcomes. | How a different action or business rule changes the records. |
| **Mission 1 — The Interview Room** | Read clues about 14 candidate classes. | How to decide what deserves a class. |
| **Mission 2 — Find the Faults** | Diagnose and repair seven diagram problems. | How to check the claims made by boxes, lines, and numbers. |
| **Learning recap and optional bonus** | Review the ideas and fix one misplaced action. | How to explain what you learned and distinguish facts from actions. |

For your first play, follow this order. The playground is practice, so you can leave it when you are ready. It has no completion requirement.

You can stop between activities. There is no time limit. We have not measured how long beginners need, so no completion-time promise is made.

## 5. A few words in everyday language

Use this table whenever a word feels unfamiliar. The app’s **Field guide** gives more examples.

| Course word | Easy meaning | Clinic example |
|---|---|---|
| **Class** | A reusable template for a kind of thing the system remembers. | Pet. |
| **Object** | One particular thing represented using a class. | Bella’s pet record. |
| **Attribute** | A fact remembered about an object. | A pet’s weight. |
| **Value** | The information currently stored in an attribute. | Bella’s recorded weight is 12 kg. |
| **Operation** | Something an object can do or have done through the model. | `beExamined()`. The empty parentheses `()` help identify an operation in the diagrams. |
| **State** | An object’s current information. | Bella’s current recorded weight after an examination. |
| **Association** | A connection between things. | An Owner owns a Pet. |
| **Multiplicity** | How many things are allowed at one end of a connection. | How many owners one pet may have. |
| **Requirement** | Something the business needs the system to do or remember. | Keep cancelled appointments and their reasons. |
| **CRC card** | A short description of a class, its responsibilities, and its collaborators. | What Pet is, what it knows, what it can do, and which other classes it works with. |

### The four relationship numbers

| Symbol | Read it as |
|---|---|
| `1` | Exactly one. |
| `0..1` | Zero or one. |
| `1..*` | One or more. |
| `0..*` | Any number, including zero. |

**Always choose ONE object first, then look across the line.** For ONE Pet, the number beside Owner tells you how many Owners are allowed for that pet.

If the example shows Bella with two owners, the rule may still be `1..*`. That means one or more owners are allowed. It does not mean every pet must have exactly two owners.

## 6. The three guided chapters

The 19 steps include the short question at the end of each chapter. Nothing advances by itself. After each action, read Pip’s explanation and continue when you are ready.

### Chapter 1 — Make a pet record

| Step | Your action | What to notice |
|---|---|---|
| 1 | Let Bella into the clinic. | Bella is one particular dog. |
| 2 | Make the Pet template. | A class can be reused for many pets. |
| 3 | Add spaces for facts. | Attributes are the facts each record can hold. |
| 4 | Create Bella’s record. | One filled record represents one object. |
| 5 | Create Max’s record. | Two objects can use the same class. |
| 6 | Examine Bella. | Her recorded weight changes from 12 kg to 13 kg. The class stays the same. |
| 7 | Answer the short question. | Tell the class apart from one pet or one fact. |

**Idea to keep:** one template can produce many separate records.

The sample examination illustrates an update to a stored value. It is not a medical simulation or a prediction of a pet’s weight.

### Chapter 2 — Follow a booking

| Step | Your action | What to notice |
|---|---|---|
| 1 | Book Bella’s appointment. | The booking exists before Bella attends. |
| 2 | Let Bella attend. | A Visit records what actually happened. |
| 3 | Rewind the example. | You are trying an alternative ending of the same sample booking. |
| 4 | Cancel the booking. | The Appointment remains, but no Visit happens in this ending. |
| 5 | Open the saved Appointment. | Its status and reason explain the cancellation. |
| 6 | Answer the short question. | Decide which information the clinic must keep. |

**Idea to keep:** a plan and an actual event can need separate records.

The rewind button is a teaching replay. It does not mean that a real clinic should erase visits that already happened.

### Chapter 3 — Connect owners and pets

| Step | Your action | What to notice |
|---|---|---|
| 1 | Connect Owner A to Bella. | A link shows an association. |
| 2 | Link Max to Owner A. | One owner can have several pets. |
| 3 | Trace from Bella to Owner. | The number beside Owner counts owners for ONE Pet. |
| 4 | Trace from Owner to the pets. | The number beside Pet counts pets for ONE Owner. |
| 5 | Allow joint ownership. | The Owner end changes to `1..*`. The Pet end stays `1..*`. |
| 6 | Answer the short question. | Identify which endpoint responds to the new rule. |

**Idea to keep:** the numbers describe what the business allows, not how many records happen to be on screen.

## 7. How to use the practice playground

After the three chapters, choose **Try the practice playground**. It lets you repeat the examples without adding points or changing your mission answers.

### Pet records

Choose **Create Bella’s record**, then **Create Max’s record**. Notice that both records come from Pet. Choose **Examine Bella** and compare her weight with the earlier value. Max’s record does not change.

Choose **Clear the sample records** to start that experiment again. This clears only the sample records in the playground. Your completed lessons, badges, and notebook remain available.

### Booking outcomes

Choose **Just booked**, **Bella attends**, or **Owner cancels**. Each button shows an alternative outcome of the same sample booking.

Compare which records exist. When Bella attends, there is an Appointment and a Visit. When the owner cancels, the Appointment keeps its cancellation information, and there is no actual Visit in that outcome.

### Ownership links

Switch between **Original: one owner per pet** and **Allow joint ownership**. Watch the links and the number beside Owner. The number beside Pet stays the same.

After each experiment, read **What to notice**. Then try saying the result in your own words.

When you are ready, choose **Start the first mission**. Playground examples return to their starting values after the page reloads. Saved course progress does not reset with them.

## 8. Mission 1 — Find the classes

A **candidate** is a word that might deserve a class. You are investigating it, not assuming it belongs.

### Step 1 — Meet Pet

Read the first clue, **Who or what are you?** Then choose **Show what it knows**. Read that clue and choose **Show what it can do**.

After all three clues, choose **Yes · it needs a class** or **No · leave it out**. Read the explanation before continuing.

For Pet, the system needs information about individual pets. Pet is a useful category, and the clinic has work to do with those records. That is why it belongs.

### Step 2 — Make a starting guess

Choose a number, then **Check my prediction**. This is a starting guess about how many of the 14 candidates belong. It is fine to be wrong. The app explains the total, and you continue to investigate why each decision fits.

### Step 3 — Interview the other candidates

Follow the same three-clue routine. Make a decision, read the reason, and choose **Meet the next candidate**.

If you are unsure, choose **Show me how to decide** or ask Pip for a hint. You can also open **Case briefing** and reread what the clinic needs.

A word can be left out for different reasons. It may be one fact about something else, another name for an existing class, one individual person, or something outside this system’s requirements. Leaving it out as a class does not always mean throwing away its information. An address can still be stored inside Owner.

### Step 4 — See what changes when the clinic needs more

Choose **Explore the new requirements**. The clinic now needs separate branch records and dated weight measurements.

Reconsider **Weight**, then **Clinic**. After each decision, choose **Continue the review**. Read the twelve unchanged decisions and choose **Keep these 12 verdicts**.

Two decisions change. Twelve stay the same. There are now nine classes out of the original fourteen candidates.

### Step 5 — Explain the reason

Choose the explanation that connects the new Clinic class to the need for separate branch information. Read the feedback. The reason is the information the system must now remember.

### Step 6 — Collect your badge

Choose **Collect Object Spotter** or **Collect your badge**. Then choose **Enter the diagram room** to begin Mission 2.

**Idea to keep:** a class earns its place because of the requirements. A noun is only a starting clue.

## 9. Mission 2 — Repair the diagram

This mission uses a supplied diagram containing seven required faults. You do not have to draw it yourself.

### Step 1 — Follow one small clue

The default view is **One clue at a time**.

1. Look at the picture.
2. Read Pip’s reminder.
3. Choose the sentence that explains what looks wrong.
4. After the diagnosis is accepted, choose a repair.
5. Look at the updated picture and read why the repair works.

For example, a class named Dr. Ramirez represents one particular person. The repair changes it to Veterinarian, a category that can represent different veterinarians.

### Step 2 — Predict the original number of faults

Choose a number and check your prediction. Count faults in the original board, including the one you already repaired. The separate optional bonus does not count toward these seven.

### Step 3 — Repair the remaining clues

Use **Next small clue** after each repair. Repeat the same routine until all seven are fixed.

You can choose **See the full diagram** to inspect the whole board. The **Inspection list** offers another way to select its elements. Some elements are already correct, and the app explains why they should stay. You can return to **One clue at a time** whenever you want more guidance.

On a small screen, the full board may need sideways scrolling inside its own panel. The guided view shows readable close-ups of the relevant part.

### Step 4 — Allow joint ownership

The new rule allows one pet to have several owners.

Start with **ONE Pet** and look across to **Owner**. Choose `1..*` at the Owner end and apply the new rule. The Pet end stays `1..*`.

### Step 5 — Explain the new number

Choose the explanation about the owners allowed for one pet. The number does not count every owner in the clinic’s database.

### Step 6 — Collect your badge and review

Collect **Model Inspector**. Choose **See what I learned** to open the learning recap. You can also open your notebook or try the optional bonus.

**Idea to keep:** every box, line, and number makes a claim about the business. Read the claim and check the requirements.

## 10. How do I know I have finished?

You have finished the two main missions when you have collected **Object Spotter** and **Model Inspector**. Finishing the repairs alone does not collect the final badge. Complete the rule change, explanation, and badge step too.

The guided adventure has 19 steps and three short checks. The playground has no finish line. It is a place to experiment.

The **learning recap** reviews four important ideas. It also suggests questions you can explain aloud or answer in your notebook. Those reflections are optional and are not marked by the app.

The **optional compartment bonus** asks where `recordTreatment()` belongs inside Treatment. Choose the operations compartment because it is an action. This bonus is separate from the seven required faults.

You can earn **555 XP** from both missions and **20 more XP** from the bonus, for a maximum of **575 XP**. The opening adventure and playground do not award XP. You do not need a high score to experiment or ask for help.

## 11. What the buttons at the top do

| Button | When to use it |
|---|---|
| **Class Quest logo** | Return to your learning path. Your completed work stays available. |
| **How to play** | See what to do in your current activity. |
| **Case briefing** | Reread the clinic story and its requirements. |
| **Field guide** | Look up a course concept or diagram symbol. |
| **Notebook** | Read collected explanations, write notes, or download your work. |
| **Settings — the gear button** | Change sound or motion, back up or restore progress, replay, or reset. |

During a mission, Pip’s hint panel provides extra help. On a smaller screen, it may appear below the activity, so scroll down if you do not see it. **How to play** remains available at the top.

A grey **Finish this step** button means something in the current step is unfinished. The message beside it tells you what is needed. In the interview, that can mean reading the remaining clues. During a repair, it can mean choosing a correction after naming the problem.

## 12. Keep your notes and progress

The app saves completed work and your notes in the current browser when that browser allows it. Your work is not automatically sent to your instructor or shared with another computer.

### Save a readable notebook

1. Choose **Notebook**.
2. Write in **Your notes** if you want to. Notes are optional.
3. Choose **Download notebook (.md)**.
4. Keep the downloaded **Class_Quest_Notebook.md** file.

The notebook includes the explanations you collected, your notes, guided-step counts, XP, badges, and optional reflection prompts. You can read it in a text editor or any Markdown viewer. If your instructor requests it, submit it through the method they specify.

### Make a progress backup

1. Choose **Settings**.
2. Choose **Back up progress**.
3. Keep **Class_Quest_Progress.json** somewhere you can find again.

A `.json` backup is a saved copy of your place in the game. You normally do not need to edit it.

Make a backup before changing computers, changing browsers, moving or renaming the HTML file, or clearing browser data. Saving in a browser is convenient, but it is not the same as keeping a separate backup file.

### Restore a backup on another browser or computer

1. Open **Class_Quest.html** there.
2. Choose **Settings → Restore a backup**.
3. Select your **Class_Quest_Progress.json** file.
4. Review the summary of the backup.
5. Choose **Restore this backup** only when it is the copy you want.

Restoring replaces the progress and notes currently in that browser. The confirmation screen lets you back up the current progress first or keep it instead.

### If selecting a file does not work

Choose **Settings → Paste a backup**. Open your `.json` backup in a text editor, copy its entire contents, and paste them into the box. Choose **Check this backup**. You will see the same review and confirmation before anything is replaced.

If the text is incomplete or the wrong kind of file, the app explains the problem and keeps your current progress.

### If a download does not start

The app displays a **Save Class_Quest_…** link. Try that link. If downloads are still blocked, open **Show file contents**, copy all the text, and save it in a plain text editor using the displayed filename and extension.

A notebook ends in `.md` and is for reading. A progress backup ends in `.json` and is for restoring your place. They are different files.

### Replay and reset are different

| Action | What it does |
|---|---|
| **Replay the motion** | Repeats the illustration without changing your progress. |
| **Review with Pip** or **Walk me through the small steps again** | Returns to the guided chapters. Completed steps show their explanations, and their motion can be replayed. Earned progress stays complete. |
| **Replay Mission 1 / Replay Mission 2** in Settings | Reopens that mission for practice. Earned XP, badges, notes, and collected explanations stay available. The same reward cannot be earned twice. |
| **Reset all progress** | Starts everything over in this browser, including notes, the guided adventure, missions, XP, and badges. The app asks you to confirm first. |

## 13. Make the app comfortable to use

To stop movement, choose the gear button at the top, then turn on **Reduce motion**. Close Settings to keep playing. The completed records, relationships, and explanations remain visible.

This preference is saved with your progress. The app also respects your device’s reduced-motion setting. Decorative movement ends after a brief introduction; the teaching actions still animate when you choose them. **Gentle sound effects** are optional and off by default. All learning information is available as text or diagrams, so sound is not needed.

You can use browser zoom to make text larger. The layout adapts to narrow screens, and the diagram lesson provides close-up views. A laptop or desktop gives the full diagram more room. On a phone, opening a downloaded HTML file depends on the phone’s browser and file app.

| Key | What it does |
|---|---|
| **Tab / Shift+Tab** | Move forward or backward through controls. |
| **Enter / Space** | Activate a focused button or diagram target. |
| **Arrow keys** | Move between candidate cards, or change a selection where arrow keys are supported. |
| **Escape** | Close a dialog, or clear a full-diagram inspection. |

There is a skip link at the start of the page. Feedback uses words and symbols as well as color. This version has been reviewed for keyboard and responsive behavior, but it has not had a formal accessibility audit or complete screen-reader study.

## 14. Common questions

| What you see | What to do |
|---|---|
| The file opens as text or a preview. | Download it and use **Open with** to choose a browser. Keep the `.html` extension. |
| Buttons do nothing. | Make sure you opened the downloaded HTML in a browser that allows JavaScript. A document preview may not run it. |
| You are not sure where to go. | Choose **How to play**. It explains the current task and next action. |
| The next button is grey. | Finish the task described beside it. Read all three clues, submit the prediction, complete the repair, or answer the explanation question as required. |
| The whole diagram looks small. | Use **One clue at a time**. On the full board, scroll within the diagram panel. |
| No sound plays. | Sound starts off. You may enable it in Settings, but it is not needed to learn. |
| Animation does not play. | Check **Settings → Reduce motion** and your device preference. The final information remains usable without animation. |
| XP does not increase during the adventure. | That is expected. The guided adventure and playground are unscored practice. |
| XP does not increase during a replay. | Each reward is earned once. Replay is for practice. |
| Progress is missing after switching devices or browsers. | Restore your `.json` backup. There is no online account or automatic sync. |
| The app says it cannot save. | Keep playing if you want, but back up before closing. Download your notebook too if you want a readable copy. |
| A backup will not restore. | Use the complete `.json` progress backup. A `.md` notebook is not a progress backup. Try **Paste a backup** if file selection is the problem. |
| You cannot find the instructor’s submission button. | The app has no automatic submission. Follow your instructor’s directions outside the game. |

## 15. Privacy and how Pip works

Pip uses prepared explanations, hints, and feedback written for this clinic case. Pip works offline. It does not connect to a live AI model or accept open-ended chat questions. Your personal notes are not automatically read or graded by AI.

The app has no accounts, analytics, ads, remote fonts, or third-party libraries. The pictures, lesson content, styles, and scripts are inside the HTML. A browser policy included in the file blocks outgoing connections and external assets.

Progress stays in the current browser. Downloaded notebooks and backups contain your notes, so share them only where you intend to. The app itself does not send them anywhere.

---

## 16. Notes for instructors

Students can start with Section 1 and the app. The sections below explain the exercise keys, assumptions, source coverage, and implementation limits.

### Suggested classroom use

Introduce the clinic problem in one sentence: **“Help this clinic decide what its software must remember.”** Ask students to begin with **Start with Pip** and work at their own pace. They can work individually or in pairs, explaining their choices aloud.

After the missions, ask one student to explain why an Appointment differs from a Visit. Ask another to read both ends of Owner–Pet aloud. Then ask why the Weight decision changes when the clinic needs dated measurements.

Students can write a short reflection in the notebook. The app offers three prompts for that purpose. You can ask them to submit the notebook if it fits your course, but the app has no instructor dashboard or automatic submission.

The guided choices help students practice the supplied case. To check independent modeling, use a separate instructor-approved case and ask students to build or explain its model. Replaying this same case is revision, not a fresh assessment after the answers are familiar.

### XP is encouragement

Wrong answers do not deduct XP. Predictions earn participation XP even when the guess differs from the key. Class decisions, repairs, and explanations must be resolved before the related step advances.

| Reward | XP each | Total available |
|---|---:|---:|
| Original candidate decisions | 10 × 14 | 140 |
| Decisions under changed requirements | 5 × 14 | 70 |
| Two predictions | 5 × 2 | 10 |
| Seven required repairs | 25 × 7 | 175 |
| Joint ownership correction | 20 | 20 |
| Two final explanations | 20 × 2 | 40 |
| Two mission badges | 50 × 2 | 100 |
| Optional compartment bonus | 20 | 20 |
| **Maximum** | | **575** |

The twelve unchanged decisions are reviewed together and award their remaining XP together on first confirmation. XP and badges are not secure grading records or proof of independent work.

## 17. Model assumptions and source reconciliations

The module brief supplies the exercise-specific answer key. The provided structural-modeling handout supplies the concepts and notation. Several choices deserve explicit documentation:

1. **Two verdict changes mean twelve unchanged.** The brief says Clinic and Weight become classes and nothing else moves, but later says ten verdicts remain unchanged. The implemented arithmetic is **2 changed, 12 unchanged, 9 classes out of 14**.
2. **Seven main faults, one separate bonus.** The sample Treatment box places `recordTreatment()` in attributes, while the brief calls this an optional eighth fault. The main board starts with that operation correctly placed at the bottom. A separate optional puzzle presents and fixes the eighth fault. The main count remains seven.
3. **The repair board is an excerpt.** Mission 1 accepts seven classes, including Visit. The supplied Mission 2 diagram omits Visit and leaves six classes after its seven repairs. The app preserves that diagram rather than inventing Visit relationships or additional answer keys. It labels the board as an excerpt, not a complete production model.
4. **Some required detail lies beyond that excerpt.** A complete model would need the cancellation reason, the Visit relationships, and further validation. These are discussed in the brief and interviews but are not extra scored faults. Anything not designated as a main fault stays unchanged.
5. **The key establishes multiplicities.** The story alone does not determine every minimum and maximum. The exercise uses the exact supplied numbers, including at least one pet per owner, one invoice for each billed treatment, and at least one treatment per invoice. It does not claim those choices fit every clinic.
6. **Scope determines Address, Clinic, and Weight.** Address is an attribute group in this exercise; other systems may legitimately model addresses as classes. A single clinic can be a class if requirements call for clinic records; merely having one instance is not a universal exclusion rule. Here, branch records are introduced only by the changed requirement. The baseline records current weight and Visit information; a longitudinal measurement history is introduced explicitly in the changed requirement.
7. **Address details are preserved without duplication.** Repair 2 deletes Address and its line and replaces Owner’s generic `address` entry with `street`, `city`, and `postcode`. It does not retain both representations of the same information.
8. **Joint ownership changes only Owner–Pet.** The number beside Owner becomes `1..*`; the number beside Pet stays `1..*`. The invoice remains linked to one billing owner, as the supplied key requires.
9. **Supplementary CRC wording is instructional.** The accepted candidates’ “knows” and “can do” responses follow the supplied CRC table. Short identity responses, changed-requirement wording, and example collaborator lists make that content usable as an interview. Collaborators are illustrative, grounded in the case, and are not additional graded keys.
10. **Course notation stays bounded.** Only association, aggregation, and generalization are taught as relationship types. A hollow endpoint triangle means generalization; a small direction indicator beside an association label is not that triangle. No composition or extra scenario has been added.

## 18. Instructor answer-check table — Mission 1

The order below is the supplied alternating lineup. “Belongs” means a class in this exercise’s model.

| Candidate | Original verdict | Reason | Expanded requirements |
|---|---|---|---|
| Pet | Belongs | Category with pet facts and actions | Belongs |
| Address | Leave out | Owner attribute/group of contact facts | Leave out |
| Appointment | Belongs | Booking that can be cancelled or rescheduled | Belongs |
| The System | Leave out | Software boundary rather than a domain record | Leave out |
| Owner | Belongs | Contact details, booking, payment | Belongs |
| Weight | Leave out | Current Pet attribute in baseline | **Belongs: dated measurements** |
| Veterinarian | Belongs | Category of vet; appointments assigned to it | Belongs |
| Dr. Ramirez | Leave out | One object, an instance of Veterinarian | Leave out |
| Invoice | Belongs | Bill with payment information | Belongs |
| Client | Leave out | Duplicate name for Owner | Leave out |
| Treatment | Belongs | Description, cost, treatment and billing work | Belongs |
| Clinic | Leave out | Branch records outside original scope | **Belongs: branch records** |
| Visit | Belongs | What happened, separate from the booking | Belongs |
| Phone Number | Leave out | Owner attribute | Leave out |
| **Totals** | **7 belong / 7 leave out** | **2 verdicts change** | **9 belong / 5 leave out** |

**Mission 1 explanation:** Clinic becomes a class because the system must now tell branches apart and store facts about each. Growth alone does not justify a class.

## 19. Instructor answer-check table — Mission 2

| Fault | Where | Required correction |
|---|---|---|
| 1 | Dr. Ramirez class | Rename to **Veterinarian**. |
| 2 | Address class and Owner–Address aggregation | Delete both; place street, city, postcode in Owner. |
| 3 | Owner–Pet multiplicities | Keep **1 beside Owner**; change **Pet to 1..***. |
| 4 | Appointment–Treatment generalization | Replace with association **results in**; **1 beside Appointment**, **0..* beside Treatment**. |
| 5 | Pet–Appointment aggregation | Replace with association **is booked for**; keep **1 beside Pet**, **0..* beside Appointment**. |
| 6 | Client class | Delete the duplicate; use Owner. |
| 7 | Supplier class | Delete it because no stated requirement calls for it. |
| Rule change | Owner–Pet | Change **Owner to 1..***; keep **Pet at 1..***. |
| Separate optional bonus | Treatment compartments | Move `recordTreatment()` into operations. |

**Mission 2 explanation:** the rule now permits one pet to be linked to more than one owner. Multiplicity describes that relationship, not the number of owners in the database.

### Corrected diagram relationships

| Class A | Relationship | Class B | Number beside A | Number beside B |
|---|---|---|---|---|
| Owner | owns, association | Pet | 1; **1..*** after joint ownership | 1..* |
| Pet | is booked for, association | Appointment | 1 | 0..* |
| Veterinarian | conducts, association | Appointment | 1 | 0..* |
| Appointment | results in, association | Treatment | 1 | 0..* |
| Invoice | bills for, association | Treatment | 1 | 1..* |
| Owner | receives, association | Invoice | 1 | 0..* |

Read every endpoint independently: the number beside Class A counts A for one B. All corrected relationships on this particular board are associations. Aggregation and generalization remain valid UML concepts, taught through Wheel–Vehicle and inheritance examples in the Field guide.

### Corrected class compartments on the repair board

| Class | Attributes | Operations |
|---|---|---|
| Owner | name, street, city, postcode, phone | bookAppointment(), payInvoice() |
| Pet | name, species, breed, dateOfBirth, weight | beExamined() |
| Appointment | date, time, reason, status | cancel(), reschedule() |
| Veterinarian | name, licenceNumber | examinePet(), giveTreatment() |
| Treatment | description, cost | recordTreatment() |
| Invoice | invoiceNumber, date, totalAmount, amountPaid | issue(), recordPayment() |

Attributes display the private `−` marker. These are the supplied excerpt’s compartments, with the designated corrections; they are not an exhaustive implementation specification.

## 20. Sources and course coverage

The clinic story, lesson scope, and answer keys come from the supplied course materials. These links are for instructors who want to trace the content. Students can complete the app without opening them.

- [Provided Google Drive folder](https://drive.google.com/drive/folders/12hLHOkJsUG8JbBghyKLQw4fjNyTKbFuo)
- [Structural-modeling module brief](https://docs.google.com/document/d/153WbVcN0LZy_5cXUez3jwW4Ocwhtukcm/edit): the clinic scenario, objectives, mission sequence, answer keys, explanations, and constraints.
- [Structural-modeling handout](https://docs.google.com/presentation/d/1uxDnNIvgiPW-A0PAHYyZsVbbxGp3juf4/edit): the concepts and notation used in the course.

| Concept from the course | Where students practice or review it |
|---|---|
| Structural models and the different views of a system | Welcome; Field guide → More modeling ideas |
| Classes, objects, current state, actions, and messages | Learn with Pip; Field guide → Class boxes and More modeling ideas |
| Attributes, operations, and visibility symbols | Class boxes; both missions; optional compartment bonus |
| Associations, aggregation, and generalization | Field guide → Relationships; Mission 2 |
| Reading numbers at the ends of relationships | Ownership chapter; playground; Field guide → Multiplicity; Mission 2 |
| Finding candidate classes and using CRC cards | Mission 1; Field guide → CRC & checks; notebook |
| Checking a model against the business story | Both missions; Field guide → CRC & checks and More modeling ideas |

The brief identifies Syed Shuva, Ph.D., UNC Greensboro, as the requesting instructor and Dennis, Wixom, and Tegarden’s *Systems Analysis and Design: An Object-Oriented Approach with UML*, 6th edition, as the accompanying textbook. The app paraphrases concepts and preserves the required clinic scenario. It does not reproduce the textbook.

The referenced earlier Quality Quest HTML and README were not present in the supplied folder. This implementation follows the reuse requirements written in the module brief; it does not claim an exact comparison with those absent files.

All clinic artwork, record cards, and diagrams are drawn inside the HTML with SVG and CSS. The app is about 256 KB and has no separate image dependencies. The UML labels and relationship numbers are defined in the code so they stay precise.

## 21. What changed after the feedback?

Version 3.2 addresses all four items in **Class_Quest Feedback.docx**.

| Feedback | Change |
|---|---|
| References to lecture slides distract from the exercise. | Removed those references from the lessons, Field guide, and notebook export. The Field guide now uses concept names, including **More modeling ideas** and **About this case**. Instructor source links remain in this README. |
| The question is above the animation, but its answer buttons are below it. | Each guided step now has one task card **below the picture**. The question or instruction sits directly above its buttons. Hints, wrong-answer clues, and the explanation appear in that same card. Playground instructions and controls are also grouped together. |
| The course introduction should be simpler. | The welcome screen uses the exact replacement paragraph supplied in the feedback. UNCG and ISM301 remain visible in the course header. |
| The prominent Pause Motion control is distracting. | Removed it from the welcome screen, guided adventure, and playground. Motion preferences remain in **Settings → Reduce motion** and follow the device’s reduced-motion preference. |

The task cards use larger answer buttons, clear spacing, and a single column of choices on phones. The original question remains visible while students read feedback. Decorative animation ends after a short introduction; students still control the teaching animations by choosing an action.

The 19 guided steps, practice playground, two missions, hints, notebook, answer keys, XP rules, and progress-backup format remain compatible with the earlier version. No new scored task has been added.

## 22. Editing the app

The delivered **Class_Quest.html** is the full source of the app. You can open it in a text editor. No build step or extra folder is required to use the delivered file.

If you are changing the teaching content, save a copy first. The following names are useful search terms inside the HTML:

| Search term | What it controls |
|---|---|
| `LABS` | Clinic story, candidates, correct answers, and repair choices. |
| `GUIDE` | Mission titles, six-step instructions, and graduated hints. |
| `MATH` | Worked explanations for corrections. |
| `ADVENTURES` | The 19 guided steps, instructions, actions, and hints. |
| `LESSONS` | The three chapter checks and their takeaways. |
| `renderAdventure`, `renderPlayground` | The task cards, prompts, choices, hints, and explanations below each scene. |
| `sceneClinic`, `linkScene`, `mobileLinkScene` | The animated clinic and ownership illustrations. |
| `renderSimpleCandidate`, `renderChangedReview` | The class interviews and the changed-requirements review. |
| `REPAIR_LESSONS`, `renderGuidedRepair` | The guided diagram repairs. |
| `diagramSVG`, `syncDiagram` | The full diagram and its updates. |
| `currentTaskHelp`, `showHowToPlay` | Help for the current activity. |
| `nextLearningAction`, `showLearningRecap` | The returning-student route and learning recap. |
| `backupForReview`, `stageBackup` | Backup validation and the restore confirmation. |
| `REWARDS`, `SAVE_KEY`, `normalize` | XP rules, browser saving, and compatible progress loading. |
| `<style>` | Colors, spacing, type sizes, animation, and responsive layouts. |

Keep the scenario, key, and explanation synchronized when changing a lesson. Verify both endpoints of any relationship you edit. The module brief asks for instructor-approved keys before adding another scenario. The current app therefore stays within the supplied clinic case.

The browser save key and backup format remain compatible with the earlier versions of Class Quest. Missing fields from older versions receive defaults. An incompatible future scenario or save format would need an intentional migration, rather than reusing old progress without checking it.

The HTML can also be served as a static page if an instructor chooses to host it. That is optional and was not part of this file delivery. An institution’s hosting and course-site settings may affect scripts and browser saving.

## 23. Review and verification

This revision was checked against each written feedback item and its accompanying screenshot. The review focused on keeping the question and its controls together, removing distracting references, simplifying the welcome text, and preserving motion accessibility.

The delivered JavaScript passed a syntax check and **10 regression scenarios**. These scenarios exercise the app’s real answer and progression handlers with browser drawing and dialogs replaced by test stubs. They are separate from the browser review.

| Check | What was verified in this revision |
|---|---|
| Feedback coverage | Exact replacement welcome paragraph; no lecture-slide references in the app or notebook export; no prominent pause controls; questions and choices together below their visual. |
| Guided learning | All 19 steps completed in the Chromium preview. Each chapter’s wrong answer and correct retry worked. Explicit help and the transition to the playground worked. |
| Mission regression | Automated handler sequences completed both missions and the bonus: 14 original decisions, 14 reviewed decisions, seven repairs, joint ownership, two badges, and 575 XP. Incorrect answers did not advance the task or deduct XP. |
| Teaching consistency | The clinic story, candidate keys, repair keys, worked explanations, guided steps, and reward values match the previous version. |
| Responsive layout | Inspected the new task card at desktop, 390-pixel phone, and 320-pixel narrow-phone widths, plus enlarged text at 200%. The reviewed screens had no page-wide horizontal overflow. |
| Motion and keyboard access | Settings remained usable from the keyboard. With Reduce motion on, Bella’s record and updated weight appeared while animation was stopped. The setting remained on after reopening the preview. |
| Field guide and exports | Opened the renamed reference topics in the browser. Automated checks confirmed every topic renders and the notebook export contains no slide references. |
| Saving and compatibility | Reopening the browser preview retained the three completed chapter checks and playground access. Automated backup checks restored notes, rewards, motion preferences, and 19 guided steps; rejected invalid data; preserved rewards during replay; and loaded older saves with defaults. |
| Offline package | One HTML file with embedded art, styles, and scripts; no external script or stylesheet dependency; outgoing connections blocked by the file’s policy. |

The browser review used a locally served Chromium preview. It does not replace checking the downloaded HTML on actual classroom devices. This revision did not repeat native file-picker import, end-to-end download delivery, Firefox, Safari, or assistive-technology testing. Export contents and restoration behavior were checked in the app logic.

The app has not had a formal accessibility audit or a study of student learning outcomes. A short session with first-time students is still the best way to check whether they can explain the ideas afterward. Technical checks alone cannot establish a perfect score or guarantee that every student will enjoy the game.

Version 3.2 · Revised September 21, 2026.
