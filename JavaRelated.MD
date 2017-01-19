@PreAuthorize("hasRole('ROLE_XYZ')") is the same as @PreAuthorize("hasAuthority('ROLE_XYZ')") and in Spring security 4 
@PreAuthorize("hasRole('XYZ')") is the same as @PreAuthorize("hasAuthority('ROLE_XYZ')").
