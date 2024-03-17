## Description 
- The backend architecture that helps run the geo-guessing game.

## Backend
### Core Functions
- *calculateDistance* : Computes the distance between two geographical coordinates using the Haversine formula, https://en.wikipedia.org/wiki/Great-circle_distance returning the result in meters.
- *generateRandomCoordinatesLimited* : Generates random geographical coordinates based on input from a random number generator [ChainlinkVRF], then identifies and returns the closest city from a predefined list, along with the distance to that city.
- *fetchGameGuessesAndFormat*: Retrieves and formats guess data for a specified game from the smart contract on the Arbitrum Sepolia network, adjusting for co-ordinate scaling.
- *findWinner*: Identifies the closest guess to a specified winning location from a set of guesses using smartcontract, determining the winner's address and their guess's proximity to the target coordinates.
- *generateImageFromCity*: Generates an image of a specified city by invoking OpenAI's DALL-E model, incorporating unique elements for a uniquely generated NFT.
