function countMonths(dateFrom, dateTo) {
    const startDate = new Date(dateFrom);
    const endDate = new Date(dateTo);

    // Calculate difference in milliseconds
    const diffTime = Math.abs(endDate - startDate);
    // Convert milliseconds to months
    const diffMonths = Math.floor(diffTime / (1000 * 60 * 60 * 24 * 30));

    return diffMonths;
}

// Example usage
const monthsBetween = countMonths('2000-01-01', '2024-08-13');
console.log(`There are ${monthsBetween} months between the two dates.`);
