---
title: "How to: run backend locally"
---

<!-- markdownlint-disable MD033 -->

# How to: run backend locally

This is if you'd like to replicate the pipeline action `the_od_bods` repo on a local machine.

It will gather fresh data from API calls and web scrapers, process them, then write prepared listings to the local JKAN repo.

## Prerequisites

To get started, you should have the following installed:

- Git
- Python 3.x
- Python Package Manager (Pip)
- Docker

## Getting started

<ol style="list-style-type: decimal;margin-left:8px;">
    <li>Have <code>the_od_bods</code> and <code>jkan</code> repos on local in the same directory<ol style="list-style-type: lower-alpha;">
            <li>`git clone</code> if it&apos;s the first time, or <code>git pull</code> to update repos</li>
            <li>you must have the <code>jkan</code> repo in local, even if you don&apos;t intend to use it, or the pipeline action will fail.</li>
        </ol>
    </li>
    <li>Run pipeline<ol style="list-style-type: lower-alpha;">
            <li>Run natively<ol style="list-style-type: lower-roman;">
                    <li>Set up or update Python environment<ol style="list-style-type: decimal;">
                            <li><code>the_od_bods</code> repo runs exclusively in python</li>
                            <li>python packages needed are specified in <code>the_od_bods/requirements.txt</code></li>
                            <li>you may use any environment manager of your choice: conda, venv, poetry or other.</li>
                        </ol>
                    </li>
                    <li>Run <code>run.sh</code><ol style="list-style-type: decimal;">
                            <li>In terminal, in <code>the_od_bods</code> execute the shell script <code>sh run.sh</code></li>
                            <li>Wait for confirmation message &ldquo;Scraping complete&rdquo;</li>
                            <li>Whole action can take ~15 minutes to complete</li>
                        </ol>
                    </li>
                    <li>Run <code>merge_data.py</code> and <code>export2.jkan.py</code><ol style="list-style-type: decimal;">
                            <li>In terminal, in the <code>the_ods_bods</code> execute the shell script <code>python merge_data.py</code></li>
                            <li>In terminal, in <code>the_od_bods</code> execute the shell script <code>python export2jkan.py</code></li>
                        </ol>
                    </li>
                </ol>
            </li>
            <li>Run using Docker<ol style="list-style-type: lower-roman;">
                    <li>Run image build
                        <ol>
                            <li>In terminal, in <code>the_od_bods</code> execute the shell script <code>docker build -t open_data_scotland_pipeline .</code></li>
                        </ol>
                    </li>
                    <li>Run image in container
                        <ol>
                            <li>In terminal, in <code>the_od_bods</code> execute the shell script <code>docker run -t --name ods_pipeline open_data_scotland_pipeline</code></li>
                        </ol>
                    </li>
                    <li>Extract container contents
                        <ol>
                            <li>To delete previous files in the JKAN directory, in terminal, from <code>jkan</code>, execute the shell script <code>rm -r _datasets/*</code></li>
                            <li>In terminal, in <code>jkan</code> to copy the JKAN files, execute the shell script <code>docker cp ods_pipeline:./usr/src/app/jkan/_datasets/ ./_datasets</code></li>
                            <li>In terminal, in <code>the_od_bods</code> to copy the pipeline files, execute the shell script <code>docker cp ods_pipeline:./usr/src/app/the_od_bods/ .</code></li>
                        </ol>
                    </li>
                </ol>
            </li>
            <li>
                To see changes in frontend see <a href="../how-to-run-frontend-locally">How to: Run frontend locally</a>
            </li>
        </ol>
    </li>
</ol>
