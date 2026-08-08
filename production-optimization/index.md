---
layout: null
title: Production Optimization | Brendan Matsumoto
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
    content="A 30-day Excel Solver production optimization case study balancing internal supply, outside sourcing, recombined milk, reserves, inventory, and storage costs."
  >

  <title>
    Production Optimization | Brendan Matsumoto
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

      <a class="brand" href="../">
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

          / Production Optimization

        </div>


        <p class="eyebrow">

          Excel Solver · Supply Planning · Graduate Project

        </p>


        <h1>

          Supply Chain Production Optimization Model

        </h1>


        <p class="project-lead">

          I built a 30-day production and sourcing model to determine
          how demand should be fulfilled through internal MAMD milk,
          outside-union supply, and recombined milk while accounting
          for reserves, inventory availability, operating costs,
          and storage requirements.

        </p>


        <div class="tag-row">

          <span class="tag">
            Excel Solver
          </span>

          <span class="tag">
            Optimization
          </span>

          <span class="tag">
            Supply Planning
          </span>

          <span class="tag">
            Inventory Balance
          </span>

          <span class="tag">
            Sourcing
          </span>

        </div>

      </section>



      <!-- KEY RESULTS -->

      <section class="section">

        <div class="kpi-grid">


          <div class="kpi">

            <strong>
              8,958,268 L
            </strong>

            <span>
              Total demand fulfilled
            </span>

          </div>


          <div class="kpi">

            <strong>
              0 L
            </strong>

            <span>
              Demand gap across the model
            </span>

          </div>


          <div class="kpi">

            <strong>
              ₹24.30M
            </strong>

            <span>
              Modeled total profit
            </span>

          </div>


          <div class="kpi">

            <strong>
              1.69M L
            </strong>

            <span>
              Outside-union supply selected
            </span>

          </div>


          <div class="kpi">

            <strong>
              18,954 L
            </strong>

            <span>
              Recombined milk selected
            </span>

          </div>


          <div class="kpi">

            <strong>
              30 Days
            </strong>

            <span>
              Planning horizon
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
                Meet demand without treating every supply source
                as interchangeable.
              </h3>

              <p>

                The model has to determine how daily demand should
                be covered when internal supply alone is not always
                enough.

                Each additional sourcing option has different cost
                and inventory implications, so the objective is not
                simply to maximize production.

                The model has to determine the most profitable
                feasible supply mix.

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
                  Optimization Modeling
                </span>

                <span class="skill">
                  Scenario Analysis
                </span>

              </div>

            </div>


          </aside>



          <!-- MAIN CASE CONTENT -->

          <div class="case-main">


            <div class="panel">

              <p class="eyebrow">
                Model Structure
              </p>


              <h2>
                How I translated the case into a decision model
              </h2>


              <ul class="clean-list">

                <li>
                  Modeled daily demand and internal raw milk supply
                  across a 30-day planning horizon.
                </li>

                <li>
                  Reserved 5% of daily raw milk and carried prior
                  reserve or opening stock into the next day's
                  available supply.
                </li>

                <li>
                  Used outside-union milk and recombined milk as
                  alternative supply sources when internal milk
                  was insufficient.
                </li>

                <li>
                  Tracked skim milk powder and butter consumption
                  required for recombined milk production.
                </li>

                <li>
                  Included opening SMP and butter inventory
                  beginning on Day 12.
                </li>

                <li>
                  Modeled butter storage with a binary activation
                  decision, 10,000 kg capacity, and a fixed daily
                  storage cost.
                </li>

                <li>
                  Set the objective to maximize total modeled
                  profit while forcing the daily demand gap
                  to zero.
                </li>

              </ul>



              <div
                class="formula-stack"
                aria-label="Core model relationships"
              >

                <div class="formula">

                  Total Production =
                  MAMD Raw Used +
                  Outside Union Milk +
                  Recombined Milk

                </div>


                <div class="formula">

                  Demand Gap =
                  Demand − Total Production = 0

                </div>


                <div class="formula">

                  Daily Profit =
                  Revenue − MAMD Cost − Outside Milk Cost
                  − Recombined Milk Cost − Storage Cost

                </div>

              </div>

            </div>



            <div class="panel">

              <p class="eyebrow">
                Decision Logic
              </p>


              <h2>
                Why the sourcing mix matters
              </h2>


              <p>

                Internal MAMD milk is the lowest-cost processed
                source in the model, so it is used first when
                available.

                Outside-union milk provides the majority of the
                remaining volume needed to close the demand gap.

                Recombined milk is more constrained because it
                consumes finite SMP and butter inventory and
                carries its own unit cost.

                The Solver model evaluates these tradeoffs
                simultaneously rather than selecting sources
                one day at a time.

              </p>

            </div>



            <div class="panel">

              <p class="eyebrow">
                Result
              </p>


              <h2>
                A feasible 30-day supply plan with zero shortages
              </h2>


              <p>

                The optimized plan fulfills all 8.96 million liters
                of modeled demand.

                The model selects approximately 1.69 million liters
                of outside-union milk and 18,954 liters of
                recombined milk while maintaining a zero cumulative
                demand gap.

                The resulting objective value is approximately
                ₹24.30 million in modeled profit.

              </p>


              <p>

                The important part of the project is not only the
                final objective value.

                The model demonstrates how sourcing, inventory,
                reserve policy, and storage constraints interact
                and converts those relationships into an auditable
                daily supply plan.

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
                  Converting a business problem into decision
                  variables, formulas, constraints, and an
                  objective function.
                </li>

                <li>
                  Building multi-period inventory and reserve
                  logic instead of treating each day independently.
                </li>

                <li>
                  Evaluating cost tradeoffs across internal
                  production, outside sourcing, and recombination.
                </li>

                <li>
                  Using a binary variable to represent a fixed-cost
                  storage decision.
                </li>

                <li>
                  Validating model feasibility through a zero
                  demand-gap check.
                </li>

                <li>
                  Turning Solver output into a daily production
                  plan that can be reviewed by an operations
                  decision-maker.
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
              Model Screenshots
            </h2>

          </div>


          <p>
            Click any screenshot to open the full-size workbook view.
          </p>

        </div>



        <div class="gallery">


          <a
            href="opt%201.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="opt%201.png"
              alt="Production optimization workbook screenshot 1"
            >

          </a>



          <a
            href="opt%202.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="opt%202.png"
              alt="Production optimization workbook screenshot 2"
            >

          </a>



          <a
            href="opt%203.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="opt%203.png"
              alt="Production optimization workbook screenshot 3"
            >

          </a>



          <a
            href="opt%204.png"
            target="_blank"
            rel="noopener"
          >

            <img
              src="opt%204.png"
              alt="Production optimization workbook screenshot 4"
            >

          </a>


        </div>

      </section>



      <!-- NEXT PROJECT -->

      <section class="section">

        <div class="contact-card">


          <div>

            <p class="eyebrow">
              Next Project
            </p>

            <h2>
              Workforce Scheduling Optimization
            </h2>

            <p>

              See how I applied the same constraint-based thinking
              to employee availability and weekly staffing decisions.

            </p>

          </div>



          <div class="project-actions">

            <a
              class="button primary"
              href="../workforce-optimization/"
            >
              View Workforce Project
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
