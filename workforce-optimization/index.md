---
layout: null
title: Workforce Scheduling Optimization | Brendan Matsumoto
---

<html lang="en">

<head>

  <meta charset="utf-8">

  <meta
    name="viewport"
    content="width=device-width, initial-scale=1"
  >

  <meta
    name="description"
    content="An Excel Solver workforce scheduling case study using employee availability, daily staffing requirements, and weekly hour constraints."
  >

  <title>
    Workforce Scheduling Optimization | Brendan Matsumoto
  </title>

  <link
    rel="stylesheet"
    href="../assets/css/portfolio.css"
  >

</head>


<body>

  <div class="portfolio-shell">


    <!-- NAVIGATION -->

    <nav class="site-nav" aria-label="Primary navigation">

      <a
        class="brand"
        href="../"
      >
        Brendan Matsumoto
      </a>


      <div class="nav-links">

        <a href="../#projects">
          Projects
        </a>

        <a href="../#experience">
          Experience
        </a>

        <a
          href="../Brendan%20Matsumoto%20Resume%20C2.pdf"
          target="_blank"
          rel="noopener"
        >
          Resume
        </a>

      </div>

    </nav>



    <main>


      <!-- PROJECT HERO -->

      <section class="project-hero">


        <div class="breadcrumb">

          <a href="../">
            Portfolio
          </a>

          / Workforce Scheduling

        </div>


        <p class="eyebrow">

          Excel Solver · Workforce Planning · Operations

        </p>


        <h1>

          Workforce Scheduling Optimization Model

        </h1>


        <p class="project-lead">

          I developed an Excel Solver scheduling model to structure
          weekly staffing decisions around employee availability,
          daily coverage requirements, per-day hour limits, and
          employee-specific weekly hour ranges.

          The portfolio version is presented as a scheduling demo
          using modeled staffing inputs.

        </p>



        <div class="tag-row">

          <span class="tag">
            Excel Solver
          </span>

          <span class="tag">
            Workforce Planning
          </span>

          <span class="tag">
            Scheduling
          </span>

          <span class="tag">
            Constraint Modeling
          </span>

          <span class="tag">
            Operations
          </span>

        </div>


      </section>



      <!-- KEY MODEL CHARACTERISTICS -->

      <section class="section">

        <div class="kpi-grid">


          <div class="kpi">

            <strong>
              7 Days
            </strong>

            <span>
              Weekly scheduling horizon
            </span>

          </div>



          <div class="kpi">

            <strong>
              5 Employees
            </strong>

            <span>
              Employees represented in the demo
            </span>

          </div>



          <div class="kpi">

            <strong>
              8 Hrs
            </strong>

            <span>
              Maximum modeled hours per employee per day
            </span>

          </div>



          <div class="kpi">

            <strong>
              Daily
            </strong>

            <span>
              Coverage requirements checked by day
            </span>

          </div>



          <div class="kpi">

            <strong>
              Weekly
            </strong>

            <span>
              Employee minimum and maximum hours
            </span>

          </div>



          <div class="kpi">

            <strong>
              Solver
            </strong>

            <span>
              Optimization-based scheduling approach
            </span>

          </div>


        </div>

      </section>



      <!-- CASE STUDY -->

      <section class="section">

        <div class="case-grid">


          <!-- SIDEBAR -->

          <aside class="case-sidebar">


            <div class="panel">

              <p class="eyebrow">
                Business Problem
              </p>


              <h3>

                A schedule has to satisfy coverage and employee
                constraints at the same time.

              </h3>


              <p>

                Manual scheduling becomes more difficult when
                employees have different availability and weekly
                hour requirements.

                The model organizes those requirements into one
                decision framework so staffing changes can be
                evaluated systematically instead of relying only
                on manual trial and error.

              </p>

            </div>



            <div class="panel">

              <p class="eyebrow">
                Tools
              </p>


              <div class="skill-cloud">

                <span class="skill">
                  Microsoft Excel
                </span>

                <span class="skill">
                  Solver
                </span>

                <span class="skill">
                  Workforce Planning
                </span>

                <span class="skill">
                  Constraint Modeling
                </span>

              </div>

            </div>



            <div class="note">

              This portfolio version is a scheduling demonstration.

              It communicates the model design and decision logic
              without presenting proprietary staffing data as a
              live production schedule.

            </div>


          </aside>



          <!-- MAIN CONTENT -->

          <div class="case-main">


            <div class="panel">

              <p class="eyebrow">
                Model Structure
              </p>


              <h2>
                How the weekly schedule is represented
              </h2>


              <ul class="clean-list">

                <li>

                  Employee-by-day cells represent scheduled hours
                  across Monday through Sunday.

                </li>


                <li>

                  Daily totals aggregate employee scheduled hours
                  and compare them with minimum staffing
                  requirements.

                </li>


                <li>

                  Each employee has an individual weekly minimum
                  and maximum hour requirement.

                </li>


                <li>

                  Employee availability is represented separately
                  so unavailable days can be restricted.

                </li>


                <li>

                  A daily maximum of eight hours limits the amount
                  assigned to one employee on one day.

                </li>


                <li>

                  The objective cell sums scheduled payroll hours
                  so Solver can search for a lower-hour feasible
                  schedule.

                </li>

              </ul>



              <div
                class="formula-stack"
                aria-label="Core scheduling relationships"
              >


                <div class="formula">

                  Daily Coverage =
                  Sum of Employee Hours Scheduled for That Day

                </div>


                <div class="formula">

                  Weekly Employee Hours =
                  Sum of Monday–Sunday Assignments

                </div>


                <div class="formula">

                  Objective =
                  Minimize Total Scheduled Payroll Hours
                  Subject to Staffing and Availability Constraints

                </div>


              </div>


            </div>



            <div class="panel">

              <p class="eyebrow">
                Decision Logic
              </p>


              <h2>

                Why this is more useful than a static schedule

              </h2>


              <p>

                The model separates operating inputs from scheduling
                decisions.

                Employee availability, daily staffing needs, and
                weekly hour ranges can be changed, and the schedule
                can then be re-optimized around the new operating
                conditions.

                That makes the workbook useful as a scenario-testing
                tool rather than a one-time schedule template.

              </p>


            </div>



            <div class="panel">

              <p class="eyebrow">
                Operational Value
              </p>


              <h2>

                A repeatable framework for staffing decisions

              </h2>


              <p>

                The output gives a manager a structured starting
                point for a weekly schedule while also displaying
                the supporting checks, including daily staffing
                totals, employee weekly totals, and availability
                logic.

                The model is designed to make staffing assumptions
                visible so a manager can understand why a schedule
                is feasible rather than receiving a black-box result.

              </p>


            </div>



            <div class="panel">

              <p class="eyebrow">
                What This Demonstrates
              </p>


              <h2>
                Skills shown in the project
              </h2>


              <ul class="clean-list">

                <li>

                  Translating operating policies into explicit
                  scheduling constraints.

                </li>


                <li>

                  Designing employee-by-day decision variables
                  that are easy for a manager to audit.

                </li>


                <li>

                  Linking employee availability data to
                  scheduling feasibility.

                </li>


                <li>

                  Balancing daily coverage with employee-specific
                  weekly hour limits.

                </li>


                <li>

                  Using Solver to support staffing decisions
                  instead of relying only on manual trial and error.

                </li>


                <li>

                  Building an operations tool that can be rerun
                  when staffing assumptions change.

                </li>


              </ul>


            </div>


          </div>


        </div>


      </section>



      <!-- SCREENSHOTS -->

      <section class="section">

        <div class="section-heading">


          <div>

            <p class="eyebrow">
              Workbook Walkthrough
            </p>

            <h2>
              Scheduling Screenshots
            </h2>

          </div>


          <p>

            Click any screenshot to open the full-size workbook view.

          </p>


        </div>



        <div class="gallery">


          <a
            href="sch%201.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="sch%201.png"
              alt="Workforce scheduling workbook screenshot 1"
            >

          </a>



          <a
            href="sch%202.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="sch%202.png"
              alt="Workforce scheduling workbook screenshot 2"
            >

          </a>



          <a
            href="sch%203.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="sch%203.png"
              alt="Workforce scheduling workbook screenshot 3"
            >

          </a>



          <a
            href="sch%204.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="sch%204.png"
              alt="Workforce scheduling workbook screenshot 4"
            >

          </a>


        </div>


      </section>



      <!-- RELATED PROJECT -->

      <section class="section">


        <div class="contact-card">


          <div>

            <p class="eyebrow">
              Related Project
            </p>

            <h2>
              Supply Chain Production Optimization
            </h2>

            <p>

              See a larger multi-period Solver model covering
              sourcing, inventory, reserves, recombination,
              storage, and modeled profitability.

            </p>

          </div>



          <div class="project-actions">

            <a
              class="button primary"
              href="../production-optimization/"
            >
              View Production Project
            </a>

            <a
              class="button"
              href="../"
            >
              Back to Portfolio
            </a>

          </div>


        </div>


      </section>


    </main>



    <footer class="footer">

      Brendan Matsumoto · Supply Chain Analytics Portfolio

    </footer>


  </div>

</body>

</html>
