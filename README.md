`mermaid
graph TD
    Start([Start]) --> InputN[/Input: Students Count/]
    InputN --> CreateArray[Create Dynamic Array]
    CreateArray --> Loop{For each Student}
    Loop -- Yes --> GetGrade[/Input Grade/]
    GetGrade --> Check{Grade > 100?}
    Check -- Yes --> Fix[Set Grade = 100]
    Fix --> Loop
    Check -- No --> Loop
    Loop -- No --> Process[Calculate Avg & Max]
    Process --> Output[/Display Results/]
    Output --> End([End])
