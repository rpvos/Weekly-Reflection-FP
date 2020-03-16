### week 3

#### samenwerking

Deze week hebben we weer een tutor gesprek gehad. hier kregen we veel
feedback over de vergadering, deze verliep niet soepel. Een van de
fouten was in de notulen bespreken en zorgen dat je aan de hand hiervan
een planning maakt.

#### mijn bijdrage

- klassendiagram bijgewerkt
  ![Klassen diagram week 3](../Resources/klassenDiagram_week3.png "Klassen
  diagram week 3")
- test cases schrijven <br> test case StartUp:

| Steps                              | Procedures                           | Expected result                                        |
|:-----------------------------------|:-------------------------------------|:-------------------------------------------------------|
| Start the application              | select the jar file and press launch | opens the schedule tab                                 |
| checks for saved shows             | -                                    | loads all the previously saved shows from the saveFile |
| load the shows in tot the viewPane | -                                    | All the shows are formatted and shown in the pane      |

test case AddShow: dependent on startUp

| Steps               | Procedures                                                                                 | Expected result                                           |
|:--------------------|:-------------------------------------------------------------------------------------------|:----------------------------------------------------------|
| open the add window | Click the Add button                                                                       | a pop-up window occurs                                    |
| Fill in the fields  | fill in the show name, begin time, end time, stage, Genre, expected population and artists | all fields can be filled in                               |
| submit              | Click the submit button                                                                    | the created show is added to the planner and the viewpane |


test case EditShow: dependent on StartUp

| Steps                | Procedures                                  | Expected result                                                            |
|:---------------------|:--------------------------------------------|:---------------------------------------------------------------------------|
| select an show       | click on one of the shows in the viewpane   | the show gets highlighted that is selected                                 |
| open the edit window | Click the Edit button                       | a pop-up window occurs                                                     |
| loading              | -                                           | load the information from the selected show and fill them in in the window |
| edit                 | now you can edit every piece of information | the data in the fields can be modified                                     |
| submit               | click the Submit button                     | the data from the pop-up window is copied on to the show if valid          |
| close window         | -                                           | closes the window after all actions are done                               |


test case RemoveShow: dependent on StartUp

| Steps                  | Procedures                                | Expected result                                                         |
|:-----------------------|:------------------------------------------|:------------------------------------------------------------------------|
| select an show         | click on one of the shows in the viewpane | the show gets highlighted that is selected                              |
| open the remove window | Click the Remove button                   | a pop-up window occurs                                                  |
| loading                | -                                         | load the information from the selected show and show them on the window |
| confirm the deletion   | click the delete button                   | deletes the show from the application                                   |
| close window           | -                                         | closes the window after all actions are done                            |


- table view automatisch data laten laden
- fixed the saving so it saves as an json file format instead of a
  objectIO file
- het laden van de json file
