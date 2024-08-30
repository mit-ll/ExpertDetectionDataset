# ExpertDetectionDataset
An easy-to-access, data-science-training dataset that contains users, posts, and identification of experts

We download 12 Forums:
  - Physics
  - Math
  - Gardening
  - Gaming
  - Fitness
  - English
  - Economics
  - Cooking
  - Board Games
  - Biology
  - Writers
  - Philosophy

For each user on the above stacks, we select their posts and put them in a list.  We also select their comments and put those in a list.  For each post or comment, we extract the text, score, and the publication time.  For each post, we also extract the type of post (question or answer).

We store this data in 3 pandas DataFrames:
  - **User_comments**: user id, list of text from comments, list of sources, list of scores, list of post times
  - **User_posts**:  user id, list of text from posts, list of sources, list of scores, list of post times, list of post types
  - **User_info**: user id, indicator whether user is an expert in physics, user’s physics reputation from StackExchange, indicator and reputation for each forum above
  
A user is identified as an *expert* if their reputation in the Stack is greater than 200. 


## Attribution
[![CC BY-SA 4.0][cc-by-sa-shield]][cc-by-sa]

The original dataset was published by Stack Exchange, Inc. on 2014-01-21 18:54:32.  The ExpertDetectionDataset is a curated and reformatted version obtained from https://archive.org/details/stackexchange under the Creative Common license CC BY-SA 4.0 

[cc-by-sa]: http://creativecommons.org/licenses/by-sa/4.0/
[cc-by-sa-image]: https://licensebuttons.net/l/by-sa/4.0/88x31.png
[cc-by-sa-shield]: https://img.shields.io/badge/License-CC%20BY--SA%204.0-lightgrey.svg

## Disclaimer
DISTRIBUTION STATEMENT A. Approved for public release: distribution unlimited.

© 2024 Massachusetts Institute of Technology.
  - Subject to FAR 52.227-11 – Patent Rights – Ownership by the Contractor (May 2014)
  - SPDX-License-Identifier: CC-BY-SA-4.0

This material is based upon work supported by the Department of the Air Force under Air Force Contract No. FA8702-15-D-0001. Any opinions, findings, conclusions or recommendations expressed in this material are those of the author(s) and do not necessarily reflect the views of the Department of the Air Force.

Delivered to the U.S. Government with Unlimited Rights, as defined in DFARS Part 252.227-7013 or 7014 (Feb 2014). Notwithstanding any copyright notice, U.S. Government rights in this work are defined by DFARS 252.227-7013 or DFARS 252.227-7014 as detailed above.

The software/firmware is provided to you on an As-Is basis
