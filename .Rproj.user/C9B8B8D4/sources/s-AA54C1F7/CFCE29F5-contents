#' palette function
#'
#' baed on functions published by Garrick Aden-Buie
#' @param primary initial color - must be in the selection
#' @param other if selection only 2 colors, the secondary color
#' @param direction whether you want ot reverse the direction of the colors
#' @keywords palette
#' @examples
#' ggplot() + my_palette(direction = -1)(2)



my_palette <- function(
  primary = "orange",
  other = "gold",
  direction = 1
) {
  stopifnot(primary %in% names(branded_colors))

  function(n) {
    if (n > 6) warning("Color Palette only has 6 colors.")

    if (n == 2) {
      other <- if (!other %in% names(branded_colors)) {
        other
      } else {
        branded_colors[other]
      }
      color_list <- c(other, branded_colors[primary])
    } else {
      color_list <- branded_colors[1:n]
    }

    color_list <- unname(unlist(color_list))
    if (direction >= 0) color_list else rev(color_list)
  }
}


