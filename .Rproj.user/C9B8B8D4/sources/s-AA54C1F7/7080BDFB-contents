#' color list
#'
#' list of custom colors for palettes


my_colors <- list(
  "orange"   = "#f06c00",
  "gold"    = "#7f0442",
  "purple" = "#edae49",
  "pink"  = "#66a182",
  "mint"   = "#2e4057",
  "grey"   = "#8d96a3"
)


#' scale_colour_matt
#'
#' This function applies my_palette
#' @examples
#' ggplot() + scale_colour_matt()


scale_colour_matt <- function(
  primary = "orange",
  other = "plum",
  direction = 1,
  ...
) {
  ggplot2::discrete_scale(
    "colour", "matts",
    branded_pal(primary, other, direction),
    ...
  )
}

#' scale_fill_matt
#'
#' This function applies my_palette
#' @examples
#' ggplot() + scale_fill_matt()

scale_fill_matt <- function(
  primary = "orange",
  other = "plum",
  direction = 1,
  ...
) {
  ggplot2::discrete_scale(
    "fill", "matts",
    branded_pal(primary, other, direction),
    ...
  )
}

