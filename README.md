# Jquery Flot Spline

## About

- Flot plugin that provides spline interpolation for line graphs
- author: Alex Bardas < alex.bardas@gmail.com >
- modified by: Avi Kohn https://github.com/AMKohn
- based on the spline interpolation described at: http://scaledinnovation.com/analytics/splines/aboutSplines.html

## Installation

- `npm install https://github.com:sergio-melendez/jquery.flot.spline`

## Usage

Example usage: (add in plot options series object)
```
		for linespline:
			series: {
				...
				lines: {
					show: false
				},
				splines: {
					show: true,
					tension: x, (float between 0 and 1, defaults to 0.5),
					lineWidth: y (number, defaults to 2),
					fill: z (float between 0 .. 1 or false, as in flot documentation)
				},
				...
			}
		areaspline:
			series: {
				...
				lines: {
					show: true,
					lineWidth: 0, (line drawing will not execute)
					fill: x, (float between 0 .. 1, as in flot documentation)
					...
				},
				splines: {
					show: true,
					tension: 0.5 (float between 0 and 1)
				},
				...
			}
```
