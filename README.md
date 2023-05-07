Download Link: https://assignmentchef.com/product/solved-operating-systems-laboratory-cs39002-assignment-3-simulation-of-cpu-scheduling-algorithms
<br>
The objective of this assignment is to evaluate various process scheduling strategies. This is achieved by generating random arrival times and CPU bursts for a set of processes following some probability distribution, and determining the performances of the chosen scheduling algorithms through simulation. The specifications for the problem are as follows.

<ol>

 <li>a) Read the number of processes N, and generate the arrival times and CPU bursts of the processes using some probability distribution. The first process is assumed to arrive at time 0; for all subsequent processes the <em>inter-arrival time</em> is generated as a random variable (between 0 and 10) following exponential distribution with some given mean. Also the CPU bursts of the processes are generated as uniform random variables (between 1 and 20). Save the generated table in a file.</li>

</ol>

<strong><em>Hint</em></strong><em>: If R is a uniform random number in the range (0, 1), a random variable from an exponential distribution with mean </em><em> can be generated as: </em>

<h1>(-1.0 /  ) * ln R</h1>

<ol>

 <li>Simulate the following CPU scheduling algorithms on the process arrival trace as generated in (a) above, and compute the average turnaround times (ATN) for the processes:

  <ul>

   <li>Non-preemptive First Come First Serve (FCFS)</li>

   <li>Non-preemptive Shortest Job First</li>

   <li>Pre-emptive Shortest Job First</li>

   <li>Round Robin with time quantum δ = 2 time units</li>

   <li>Highest response-ratio next (HRN)</li>

  </ul></li>

 <li>Run the simulation for N = 10, 50 and 100, ten times for each value of N using a shell script (bash/python), and generate the plot comparing the average values of ATN obtained for various scheduling techniques for different values of N.</li>

 <li>For FCFS (non-preemptive) determine the theoretically expected lower bound on the turn-around time and check whether that is satisfied by your simulation.</li>

</ol>

<strong>Submission Guideline:</strong>

 Create the program as a single file as <strong>a3_&lt;groupno&gt;.c</strong> or <strong>.cpp</strong>. Create the plot file as <strong>a3_plot_&lt;groupno&gt;.pdf</strong> . Upload the two files.

<strong>Evaluation Guidelines: </strong>

While entering marks, the partwise break up should also be entered according to the marking guidelines given below. There is a separate component for individual assessment, based on how the student answers questions.

<table width="435">

 <tbody>

  <tr>

   <td width="26"><strong>Sl</strong></td>

   <td width="363"><strong>Items</strong></td>

   <td width="46"><strong>Marks</strong></td>

  </tr>

  <tr>

   <td width="26"><strong>(a)</strong></td>

   <td width="363">Random number generation (uniform, exponential)</td>

   <td width="46">8</td>

  </tr>

  <tr>

   <td width="26"><strong>(b)</strong></td>

   <td width="363">Maintaining job queues for scheduling</td>

   <td width="46">8</td>

  </tr>

  <tr>

   <td width="26"><strong>(c)</strong></td>

   <td width="363">Simulation of five scheduling strategies</td>

   <td width="46">15</td>

  </tr>

  <tr>

   <td width="26"><strong>(d)</strong></td>

   <td width="363">Generation of results and plots</td>

   <td width="46">15</td>

  </tr>

  <tr>

   <td width="26"><strong>(e)</strong></td>

   <td width="363">Shell script for running the jobs</td>

   <td width="46">4</td>

  </tr>

  <tr>

   <td width="26"><strong>(f)</strong></td>

   <td width="363">Theoretical analysis of FCFS</td>

   <td width="46">5</td>

  </tr>

  <tr>

   <td width="26"> </td>

   <td width="363"><strong>Total</strong></td>

   <td width="46">55</td>

  </tr>

 </tbody>

</table>


