<!-- Add styles for alternating row colors and borders -->
<style>
  .schedule-table {
    border-collapse: separate;
    border-spacing: 0;
    table-layout: fixed;
    width: 100%;
    text-align: center;
    border: 1px solid rgba(128, 128, 128, 0.55);
    border-radius: 8px;
    overflow: hidden;
    font-size: 0.95rem;
  }

  .schedule-table th,
  .schedule-table td {
    border: 1px solid rgba(128, 128, 128, 0.3);
    padding: 10px 8px;
    word-wrap: break-word;
  }

  /* Header row: plain, just bold text — no fill color */
  .schedule-table thead th {
    font-weight: 700;
    white-space: nowrap;
  }

  /* Week column: bold only, vertically centered */
  .schedule-table .schedule-week-num {
    font-weight: 700;
    vertical-align: middle;
  }

  /* Holiday / no-class rows: recede via italics, no background needed */
  .schedule-table td[colspan="4"] {
    font-style: italic;
    opacity: 0.7;
  }
</style>


<!-- Add a jump-to button to navigate to the current week -->
<p>
  <a href="#week1">Jump to Current Week</a>
</p>

<!-- Week 1 Calendar -->
<table class="table table-bordered schedule-table" id="week1">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 1</td>
      <th>Mon 8/24</th>
      <td colspan="4">No class</td>
    </tr>
    <tr>
      <th>Tue 8/25</th>
      <td colspan="4">No class</td>
    </tr>
    <tr>
      <th>Wed 8/26</th>
      <td>
        Lec 1. Welcome + Abstraction<br/>
        (Video) <a href="https://drive.google.com/file/d/1dUlUg_4BUZrQ-t0aKLIFu9f2e3nh-gzQ/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"><a href="https://cs10.org/fa26/labs/lab01/">Lab 1. Welcome to Snap!</a> <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 8/27</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 8/28</th>
      <td>
        Talk 1. Fun "Ask me anything", abstraction, using Snap!<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 1. Welcome to CS 10! </td>
      <td></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 2 Calendar -->
<table class="table table-bordered schedule-table" id="week2">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 2</td>
      <th>Mon 8/31</th>
      <td>
        Lec 2. Functions<br/>
        (Video) <a href="https://drive.google.com/file/d/1xiNfvA8PbKNc-VAMd2YaB7X93UuJHfB6/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 2. Build Your Own Blocks <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 9/1</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 9/2</th>
      <td>
        Lec 3. Abstraction II<br/>
        (Video) <a href="https://drive.google.com/file/d/1w3ck5J-VOj6Tan7eKdhgN8OwwiD9a4Zu/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 3. Conditionals, Reporters, & Testing <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 9/3</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 9/4</th>
      <td>
        Talk 2. Making functions<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 2. Number Rep & Control Structures </td>
      <td><b>Proj 1: Wordle™ Lite Released</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 3 Calendar -->
<table class="table table-bordered schedule-table" id="week3">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 3</td>
      <th>Mon 9/7</th>
      <td colspan="4">No class (holiday)</td>
    </tr>
    <tr>
      <th>Tue 9/8</th>
      <td></td>
      <td>No Lab</td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 9/9</th>
      <td>
        Lec 4. Computing in Education<br/>
        (Video) <a href="https://drive.google.com/file/d/1BKQ0jP7T1YgsMpJ-wAJ7ZR_cd132BlYi/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Project 1 Party <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 9/10</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 9/11</th>
      <td>
        Talk 3. All Quest practice except for Iteration, Boolean, HOF<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 3. Domain/Range, Scoping, Iteration, Lists </td>
      <td></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 4 Calendar -->
<table class="table table-bordered schedule-table" id="week4">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 4</td>
      <th>Mon 9/14</th>
      <td>
        Lec 5. Iteration<br/>
        (Video) <a href="https://drive.google.com/file/d/13dQEitJYlz1EBnlLgIeMmiJ7_G8w5ncc/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 4. Iteration <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 9/15</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 9/16</th>
      <td>
        Lec 6. Lists, Scoping, & HOFs<br/>
        (Video) <a href="https://drive.google.com/file/d/1pHeJkMcS4hex5l5hfZ0DxoWpl0zwGybx/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 5. Lists & HOFs <br/> </td>
      <td></td>
      <td><b>Proj 1 Due</b></td>
    </tr>
    <tr>
      <th>Thu 9/17</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 9/18</th>
      <td>
        Talk 4. (Practice Quest) Booleans + Iteration<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc. 4: HOFs + Iteration </td>
      <td></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 5 Calendar -->
<table class="table table-bordered schedule-table" id="week5">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 5</td>
      <th>Mon 9/21</th>
      <td>
        Lec 7. Higher-Order Functions<br/>
        (Video) <a href="https://drive.google.com/file/d/1pohZVsm_LXNdiQscTqqWox3Hv8Wd6e0J/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 6. Functions as Data, HOFs <br/> </td>
      <td></td>
      <td><b>Proj 2: Spelling Bee Released</b></td>
    </tr>
    <tr>
      <th>Tue 9/22</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 9/23</th>
      <td>
        Lec 8. Algorithms<br/>
        (Video) <a href="https://drive.google.com/file/d/1eGe_LL8JUu0iNGoxfAxNxDCMX7-qcAgp/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Catch-up (optional) <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 9/24</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 9/25</th>
      <td>
        Talk 5. Quest 1 Preview<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc. 5 HOFs + Quest Review </td>
      <td><b>QUEST 1</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 6 Calendar -->
<table class="table table-bordered schedule-table" id="week6">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 6</td>
      <th>Mon 9/28</th>
      <td>
        Lec 9. Algorithmic Complexity<br/>
        (Video) <a href="https://drive.google.com/file/d/1-e_TRoFaZAZXtt1gSPLcjGmeN36Uxqnm/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 7. Algorithms <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 9/29</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 9/30</th>
      <td>
        Lec 10. Testing + 2048<br/>
        (Video) <a href="https://drive.google.com/file/d/1ajYTduj9Rpv19rZO6TSlcuQ21yBFsuy3/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 8. Testing + 2048 <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 10/1</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 10/2</th>
      <td>
        Talk 6. Quest 1 Review<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 6. HOFs, Lambdas, Debugging </td>
      <td><b>Proj 2 Due</b><br/><b>QUEST 2</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 7 Calendar -->
<table class="table table-bordered schedule-table" id="week7">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 7</td>
      <th>Mon 10/5</th>
      <td>
        Lec 11. Recursion I (Functional)<br/>
        (Video) <a href="https://drive.google.com/file/d/1rhyfIfPyb5HsSB9N8dOA_Pn58sr0yvvU/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 9. Boards <br/> </td>
      <td></td>
      <td><b>Proj 3: 2048 Released</b></td>
    </tr>
    <tr>
      <th>Tue 10/6</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 10/7</th>
      <td>
        Lec 12. Recursion II (Fractals)<br/>
        (Video) <a href="https://drive.google.com/file/d/1qb_ixaZvzDitH-eATGfOSaovxeaJaVXa/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 10. Trees & Fractals <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 10/8</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 10/9</th>
      <td>
        Talk 7. Quest 2 Review<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 7. Recursion I </td>
      <td><b>QUEST 3</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 8 Calendar -->
<table class="table table-bordered schedule-table" id="week8">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 8</td>
      <th>Mon 10/12</th>
      <td>
        Lec 13. Recursion III (Count Change)<br/>
        (Video) <a href="https://drive.google.com/file/d/1LOBsTelQjBgY0QfpdYokovIxQ3_SDHfE/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 11. Recursive Reporters <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 10/13</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 10/14</th>
      <td>
        Lec 14. Social Implications of Computing: Privacy<br/>
        (Video) <!--<a href="">(Slides)</a>-->(Slides)
      </td>
      <td rowspan="2"> Lab 12. Algorithmic Complexity <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 10/15</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 10/16</th>
      <td>
        Talk 8. Recursion III<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 8. Algorithmic Complexity + Tree Recursion </td>
      <td></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 9 Calendar -->
<table class="table table-bordered schedule-table" id="week9">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 9</td>
      <th>Mon 10/19</th>
      <td>
        Lec 15. Kathy Yelick "Saving the World with Computing"<br/>
        (Video) <a href="https://drive.google.com/file/d/1k3hl9mOVuNLAh9LzrZNGpzKaH69BwII2/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Practice Midterm (no code) <br/> </td>
      <td></td>
      <td><b>Proj 3: Due</b></td>
    </tr>
    <tr>
      <th>Tue 10/20</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 10/21</th>
      <td>
        Lec 16. HCI (Shm Almeda)<br/>
        (Video) <!--<a href="">(Slides)</a>-->
      </td>
      <td rowspan="2"> Practice Midterm (fractal) <br/> </td>
      <td></td>
      <td><b>Proj 4: Explore Released</b></td>
    </tr>
    <tr>
      <th>Thu 10/22</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 10/23</th>
      <td>
        Talk 9. Midterm 1 Preview<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 9. Midterm Preview </td>
      <td><b>MIDTERM 1</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 10 Calendar -->
<table class="table table-bordered schedule-table" id="week10">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 10</td>
      <th>Mon 10/26</th>
      <td>
        Lec 17. Concurrency<br/>
        (Video) <a href="https://drive.google.com/file/d/1nxDs9G9eijscPh4PW7Cmme7dQgMo3SUX/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 13. Concurrency <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 10/27</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 10/28</th>
      <td>
        Lec 18. OOP in Snap!<br/>
        (Video) <a href="https://drive.google.com/file/d/1tIn-P8b1ZADGqX7yZ-VzrslA-dnOzlgF/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 14. OOP in Snap! <br/> </td>
      <td></td>
      <td><b>Proj 4 Due</b></td>
    </tr>
    <tr>
      <th>Thu 10/29</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 10/30</th>
      <td>
        Talk 10. Midterm 2 Review<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 10. Proj 4 Presentations </td>
      <td><b>Final Projects Released</b><br/><b>MIDTERM 2</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 11 Calendar -->
<table class="table table-bordered schedule-table" id="week11">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 11</td>
      <th>Mon 11/2</th>
      <td>
        Lec 19. Python I - Intro<br/>
        (Video) <a href="https://drive.google.com/file/d/1k4g6eWTP0WoWxxgpx9fsBooxRhTpSoMM/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 15. Welcome to Python <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 11/3</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 11/4</th>
      <td>
        Lec 20. Python II - Data Types & Structures<br/>
        (Video) <a href="https://drive.google.com/file/d/1Yd5uJC6QNdYuhprWArCrVqRLbqDmtopK/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 16. Lists and Mutability <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 11/5</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 11/6</th>
      <td>
        Talk 11. Midterm 3 Review<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 11: Welcome to Python </td>
      <td><b>Proj 4 Comments Due</b><br/><b>Proj 4 Makeup Presentations Due</b><br/><b>Final Project Proposals Due</b><br/><b>MIDTERM 3</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 12 Calendar -->
<table class="table table-bordered schedule-table" id="week12">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 12</td>
      <th>Mon 11/9</th>
      <td>
        Lec 21. Programming Paradigms<br/>
        (Video) <a href="https://drive.google.com/file/d/1YvQDjtZSyw2tiN8uBqwxTgbZ3MIGRC_H/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 17. Data Structures in Python <br/> </td>
      <td></td>
      <td><b>Final Project Meetings</b></td>
    </tr>
    <tr>
      <th>Tue 11/10</th>
      <td></td>
      <td></td>
      <td><b>Final Project Meetings</b></td>
    </tr>
    <tr>
      <th>Wed 11/11</th>
      <td colspan="4">No class (holiday)</td>
    </tr>
    <tr>
      <th>Thu 11/12</th>
      <td></td>
      <td> Lab 18. Text Processing in Python <br/> </td>
      <td></td>
      <td><b>Final Project Meetings</b></td>
    </tr>
    <tr>
      <th>Fri 11/13</th>
      <td>
        Talk 12. Python live coding<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 12: Data Structures in Python + Concurrency </td>
      <td><b>Final Project Meetings</b><br/><b>Project 4 Resubmissions Due</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 13 Calendar -->
<table class="table table-bordered schedule-table" id="week13">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 13</td>
      <th>Mon 11/16</th>
      <td>
        Lec 22. Gen AI<br/>
        (Video) <a href="https://drive.google.com/file/d/1W5s73SjKPawZgR2nazuYorUp7tc_BUYs/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 19. Data Science <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 11/17</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 11/18</th>
      <td>
        Lec 23. Ethics in AI<br/>
        (Video) <a href="https://drive.google.com/file/d/1ibFKElf1ZtS0ChdCMIzwRbRhLODp7A3x/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Practice Postterm <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 11/19</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 11/20</th>
      <td>
        Talk 13. POSTTERM 1 PREVIEW<br/>
        (Video)<br/>
      </td>
      <td></td>
      <td> Disc 13: Postterm Practice </td>
      <td><b>POSTTERM 1</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 14 Calendar -->
<table class="table table-bordered schedule-table" id="week14">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 14</td>
      <th>Mon 11/23</th>
      <td>
        Lec 24. Python III - Game Theory<br/>
        (Video) <a href="https://drive.google.com/file/d/1_cZHoz-5i-RRs2v79vaV03udf6RiFc6o/view?usp=drive_link">(Slides)</a>
      </td>
      <td rowspan="2"> Lab 20. Linear Recursion in Python <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 11/24</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 11/25</th>
      <td colspan="4">No class (holiday)</td>
    </tr>
    <tr>
      <th>Thu 11/26</th>
      <td colspan="4">No class (holiday)</td>
    </tr>
    <tr>
      <th>Fri 11/27</th>
      <td colspan="4">No class (holiday)</td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Week 15 Calendar -->
<table class="table table-bordered schedule-table" id="week15">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 15</td>
      <th>Mon 11/30</th>
      <td>
        Lec 25. Alumni Panel<br/>
        (Video) (Slides)
      </td>
      <td rowspan="2"> Lab 21 OPTIONAL. Snap + Python Libraries <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Tue 12/1</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 12/2</th>
      <td>
        Lec 26. Conclusion and Farewell<br/>
        (Video) (Slides)
      </td>
      <td rowspan="2"> Project Work Session <br/> </td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 12/3</th>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 12/4</th>
      <td>
        Talk 14. POSTTERM 1 REVIEW<br/>
        (Video)
      </td>
      <td></td>
      <td> Disc 15: Postterm Review </td>
      <td><b>POSTTERM 2</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- RRR Week Calendar -->
<table class="table table-bordered schedule-table" id="rrrweek">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 16<br/>(RRR Week)</td>
      <th>Mon 12/7</th>
      <td>
        POSTTERM 2 REVIEW<br/>
        (Video)
      </td>
      <td></td>
      <td></td>
      <td><b>Final Project Due</b></td>
    </tr>
    <tr>
      <th>Tue 12/8</th>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 12/9</th>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 12/10</th>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 12/11</th>
      <td></td>
      <td></td>
      <td></td>
      <td><b>POSTTERM 3</b></td>
    </tr>
  </tbody>
</table>

<br/>

<!-- Finals Week Calendar -->
<table class="table table-bordered schedule-table" id="finalsweek">
  <colgroup>
    <col style="width: 7%;">
    <col style="width: 9%;">
    <col style="width: 28%;">
    <col style="width: 20%;">
    <col style="width: 20%;">
    <col style="width: 16%;">
  </colgroup>
  <thead>
    <tr>
      <th class="center schedule-week-num">Week</th>
      <th>Date</th>
      <th>Lecture</th>
      <th>Lab</th>
      <th>Discussion</th>
      <th>Assignment / Exam</th>
    </tr>
  </thead>
  <tbody class="content">
    <tr>
      <td class="schedule-week-num" rowspan="5">Week 17<br/>(Finals Week)</td>
      <th>Mon 12/14</th>
      <td></td>
      <td></td>
      <td></td>
      <td><b>Release Grades</b><br/><b>Final Project Regrades</b></td>
    </tr>
    <tr>
      <th>Tue 12/15</th>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Wed 12/16</th>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Thu 12/17</th>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
    <tr>
      <th>Fri 12/18</th>
      <td></td>
      <td></td>
      <td></td>
      <td></td>
    </tr>
  </tbody>
</table>

<br/>
