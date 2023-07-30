# task-3
import java.util.Scanner;

class Resume {
    private String name;
    private String email;
    private String phone;
    private String summary;
    private String education;
    private String experience;

    // Constructor, getters, and setters

    public String getName() {
        return name;
    }

    public void setName(String name) {
        this.name = name;
    }

    public String getEmail() {
        return email;
    }

    public void setEmail(String email) {
        this.email = email;
    }

    public String getPhone() {
        return phone;
    }

    public void setPhone(String phone) {
        this.phone = phone;
    }

    public String getSummary() {
        return summary;
    }

    public void setSummary(String summary) {
        this.summary = summary;
    }

    public String getEducation() {
        return education;
    }

    public void setEducation(String education) {
        this.education = education;
    }

    public String getExperience() {
        return experience;
    }

    public void setExperience(String experience) {
        this.experience = experience;
    }
}

public class ResumeBuilder {
    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);

        System.out.println("Welcome to the Online Resume Builder!");
        System.out.println("Please enter your details:");

        System.out.print("Name: ");
        String name = scanner.nextLine();

        System.out.print("Email: ");
        String email = scanner.nextLine();

        System.out.print("Phone: ");
        String phone = scanner.nextLine();

        System.out.print("Summary: ");
        String summary = scanner.nextLine();

        System.out.print("Education: ");
        String education = scanner.nextLine();

        System.out.print("Experience: ");
        String experience = scanner.nextLine();

        // Create the resume
        Resume resume = new Resume();
        resume.setName(name);
        resume.setEmail(email);
        resume.setPhone(phone);
        resume.setSummary(summary);
        resume.setEducation(education);
        resume.setExperience(experience);

        // Display the generated resume
        System.out.println("\nYour Resume:");
        System.out.println("Name: " + resume.getName());
        System.out.println("Email: " + resume.getEmail());
        System.out.println("Phone: " + resume.getPhone());
        System.out.println("Summary: " + resume.getSummary());
        System.out.println("Education: " + resume.getEducation());
        System.out.println("Experience: " + resume.getExperience());

        scanner.close();
    }
}
