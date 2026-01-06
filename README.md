# home-assingment-code-
home assingment code 
def normalize_company_name(company_name: str) -> str:
    """
    Normalize company name variations to the standard format:
    'CAF SoftSol India Pvt Ltd.'
    """
    # Convert to lowercase for uniform comparison
    name = company_name.lower().strip()
    
    # Define possible variations
    variations = [
        "caf softsol",
        "caf solution",
        "caf softsolution india pvt limited"
    ]
    
    # Check if the input matches any known variation
    if any(var in name for var in variations):
        return "CAF SoftSol India Pvt Ltd."
    
    # Default return if no match found
    return company_name
