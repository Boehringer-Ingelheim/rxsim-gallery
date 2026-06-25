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

# Brand palette + minimal theme for all ggplot2 output in this project
if (requireNamespace("ggplot2", quietly = TRUE)) {
  .brand <- c("#e18600", "#076d7e", "#00E47C", "#08312A", "#86251b", "#5d4495")
  options(ggplot2.discrete.colour = .brand, ggplot2.discrete.fill = .brand)
  ggplot2::theme_set(
    ggplot2::theme_minimal() +
      ggplot2::theme(
        plot.background  = ggplot2::element_rect(fill = "#F6F5F3", colour = NA),
        panel.background = ggplot2::element_rect(fill = "#F6F5F3", colour = NA)
      )
  )
}
