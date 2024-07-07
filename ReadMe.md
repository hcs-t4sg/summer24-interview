# Intro
There is some important decisions that have been made that should be kept in mind with all of this data.
*

## Data Preprocessing
1. The values for `Duration (Semesters)` and `Current Member?` were done by hand so there are possible errors that we should account for.
2. The `Duration (Semesters)` isn't based on number of projects they've done, etc. It is purely if they attended the fall/spring. This means that if an individual attended/hosted anything over the summer or winter those weren't counted in the `Duration (Semesters)`.
3. The `Current Member?` column is true if the individual was present in Spring 2024. This gives no guarantees for the future, which should be taken into account.
4. The `SWE R2 Status` column is not merely a binary. This is due to entries with `Maybe` and `Waitlist/Strong Maybe`. As a result, for it is based on the following scale:
  - `Yes` = 3
  - `Waitlist/Strong Maybe` = 2
  - `Maybe` = 1
  - `No` = 0
