# Use more CPU cores while building packages
options(Ncpus = parallel::detectCores())

# Use PPM and {pak} with {renv}
# https://github.com/rstudio/renv/
# https://github.com/r-lib/pak
options(renv.config.pak.enabled = TRUE)

# activate renv
source("renv/activate.R")

# Use the same RSPM snapshot as rxsim for reproducibility
options(repos = c(RSPM = "https://packagemanager.posit.co/cran/2026-04-11"))
