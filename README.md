# # Mini Project - Jenkins Pipeline Job (Local Setup)

## Project Overview
This project automates a CI/CD pipeline using a Jenkins Pipeline job (`My pipeline job`). It connects to `https://github.com/westgrin/jenkins-scm`, builds a Docker image, runs an Nginx container on port 8081, and uses a GitHub webhook for automatic builds. Executed on WSL Ubuntu with VS Code and Git Bash.

## Setup
- Initiated on Jul 05, 2025, 12:12 PM EDT.
- Used WSL Ubuntu, VS Code, and Git Bash in `C:\Users\Abraham\Documents\Workspace\Jenkins_Pipeline_Job`.

## Execution Steps
1. **Verify Jenkins and Install Docker**:
   - Confirmed Jenkins running on `http://localhost:8080` and installed Docker via `docker.sh`.
   - [Screenshot: `jenkins_status_pipeline_local.png` - Shows Jenkins status.]
   - [Screenshot: `docker_status_local.png` - Shows Docker status.]
2. **Update GitHub Repository**:
   - Added `Dockerfile` and `index.html` to `jenkins-scm`.
   - [Screenshot: `github_scm_files_local.png` - Shows GitHub repository files.]
3. **Create Pipeline Job**:
   - Created `My pipeline job`, configured SCM and webhook trigger, and wrote pipeline script.
   - [Screenshot: `pipeline_job_config_local.png` - Shows job configuration.]
   - [Screenshot: `pipeline_trigger_config_local.png` - Shows trigger settings.]
   - [Screenshot: `pipeline_script_local.png` - Shows pipeline script.]
4. **Run and Test Pipeline**:
   - Ran pipeline, tested webhook, and accessed Nginx on `http://localhost:8081`.
   - [Screenshot: `pipeline_build_output_local.png` - Shows build output.]
   - [Screenshot: `pipeline_webhook_output_local.png` - Shows webhook-triggered output.]
   - [Screenshot: `nginx_output_local.png` - Shows browser output.]
5. **Side Hustle Task**:
   - Created `SideHustlePipeline`, ran build, and tested webhook.
   - [Screenshot: `sidehustle_pipeline_output_local.png` - Shows pipeline output.]
   - [Screenshot: `sidehustle_webhook_output_local.png` - Shows webhook-triggered output.]

## Learning Summary
This project deepened my understanding of Jenkins Pipeline jobs for CI/CD automation. I learned to script a pipeline with declarative syntax, integrate with GitHub, and automate Docker image builds and container deployment. Using ngrok for webhook testing and resolving Docker permissions (`usermod -aG docker jenkins`) were key takeaways. The side hustle task reinforced pipeline creation and automation, enhancing my DevOps skills for streamlined workflows.

## Tools Used
- **WSL Ubuntu Terminal**: For Jenkins, Docker, and Git commands.
- **VS Code**: For editing `README.md` and `Dockerfile`.
- **Git Bash**: For GitHub operations.
- **Jenkins**: For pipeline automation.
- **Docker**: For building and running containers.
- **ngrok**: For webhook testing.

## Project Deliverables
- **Documentation**: This `README.md` with steps and learning summary.
- **Screenshots**:
  - `jenkins_status_pipeline_local.png`
  - `docker_status_local.png`
  - `github_scm_files_local.png`
  - `pipeline_job_config_local.png`
  - `pipeline_trigger_config_local.png`
  - `pipeline_script_local.png`
  - `pipeline_build_output_local.png`
  - `pipeline_webhook_output_local.png`
  - `nginx_output_local.png`
  - `sidehustle_pipeline_output_local.png`
  - `sidehustle_webhook_output_local.png`
- **Script Link**: [GitHub Repository](https://github.com/westgrin/Jenkins_Pipeline_Job)

## Troubleshooting
- Fixed `No such remote 'origin'` by adding `git remote add origin https://github.com/westgrin/Jenkins_Pipeline_Job.git`.
- Resolved Docker permissions with `usermod -aG docker jenkins`.
- Used ngrok for local webhook testing.

## Conclusion
This project successfully automated a CI/CD pipeline with Jenkins, Docker, and GitHub, serving an Nginx page on `http://localhost:8081`. The side hustle task strengthened my pipeline automation skills, preparing me for advanced DevOps practices.