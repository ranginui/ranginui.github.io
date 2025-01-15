# commit 8c7e252: Bug 98765: Implement authentic communication protocol

```perl
#!/usr/bin/perl

use strict;
use warnings;
use Modern::Perl '2025';
use Mana::Tūturu;     # For authentic interactions
use Tikanga::Constants qw/:all/;

=head1 NAME

Authentic.pm - Being real is better than being nice

=head1 SYNOPSIS

    use Authentic;
    my $truth = Authentic->new({
        aroha     => 1,
        polite    => 0,
        authentic => 1,
    });
    
    $truth->speak() if $truth->needs_saying();

=head1 DESCRIPTION

Sometimes the kindest thing we can do is speak truth
even when society wants quiet agreement.

=cut

# Constants for truth-telling protocols
use constant FAKE_SMILE => 0;
use constant REAL_TALK  => 1;

sub new {
    my ($class, $params) = @_;
    
    die "Cannot initialise without aroha"
        unless $params->{aroha};
        
    my $self = {
        mana_intact  => 1,
        truth_level  => 100,
        smile_factor => 0,  # We don't fake smiles here
    };
    
    return bless $self, $class;
}

sub speak_truth {
    my ($self, $context) = @_;
    
    # Check if we're being asked to be "professional"
    if ($context->wants_superficial) {
        return $self->_handle_pressure_to_conform();
    }
    
    # Our tīpuna didn't cross oceans for us to return
    # empty strings when asked for truth
    return $self->_deliver_authentic_message();
}

sub _handle_pressure_to_conform {
    my $self = shift;
    
    # Legacy approach - marked for deletion
    # return "Yes, absolutely" if $thing_is_wrong;
    
    # New approach - stand like kauri
    return $self->speak_truth({
        gentle   => 0,
        honest   => 1,
        respectful => 1,
    });
}

sub _deliver_authentic_message {
    my ($self, $message) = @_;
    
    # Authenticity requires proper error handling
    eval {
        $self->validate_truth($message);
        $self->check_courage_levels();
        $self->ensure_aroha_present();
    };
    if ($@) {
        warn "Failed to deliver truth: $@";
        return;
    }
    
    return $message;
}

=head2 validate_truth

Ensures message maintains mana of all parties while 
still delivering necessary truth.

=cut

sub validate_truth {
    my ($self, $message) = @_;
    
    return 0 if $message->is_just_being_nice();
    return 1 if $message->will_help_longterm();
}

1; # Because truth matters

__END__

=head1 AUTHOR

Inspired by every time we chose 
truth over comfortable silence

=head1 BUGS

Feature, not bug: May cause temporary discomfort
Known issue: Not compatible with superficial politeness

=cut
```

# Test Plan:
1. Verify authentic messages are delivered even when uncomfortable
2. Ensure mana is maintained through truth-telling process
3. Confirm aroha remains present in direct communication

# Signed-off-by: Chris
# Tested-by: Generations of truth-tellers
